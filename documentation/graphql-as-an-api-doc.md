# GraphQL as an API Doc

Make use of `@mock` directive for mocked APIs, list down the potential propagated errors, add a short description to the fields if necessary. For example:

```graphql
"""
This is a sample
"""
type Account {
  """
  Add documentation, if necessary. 
  """
  name: String!
  """
  Additional details to take note of
  """
  username: String!
}

type UpdateMeResponse {
  """
  Newly updated account
  """
  account: Account!
}

input UpdateMeInput {
  """
  It requires an email verification
  """
  email: String
  
  """
  It requires a phone number OTP
  """
  phoneNumber: String
}

type Query {
  """
  Checks the current user's details.
  
  ### Error Codes
  - \`A00001\` - <Error summary>
  """
  me: Account @mock
  
  """
  To check other accounts. 
  
  Please use \`Query.me\` if you want to check the current user's details.
  
  ### Error Codes
  - \`A00002\` - <Error sumamry>
  """
  account(id: ID!): Account @mock
}

type Mutation {
  """
   ### Error Codes
   - \`A00003\` - Invalid email
   - \`A00004\` - Invalid phone number
  """
  updateMe(input: UpdateMeInput!): UpdateMeResponse!
}
```

Add comments to add more clarity to the fields. For example:

```graphql
enum CoinDropStatus {
  """
  CoinDrop is waiting for transfer confirmation.
  """
  PENDING
  """
  CoinDrop is active and can be claimed.
  """
  ACTIVE
  """
  CoinDrop is inactive. The current time is outside the start time and end time.
  """
  INACTIVE
  """
  A maximum number of claims is reached.
  """
  EXHAUSTED
}
```
