###### Documenting Functions

##logout()

The Logout method logs out the current user.

**Parameters**

This method has no parameter.

##getNumberFriends()

Returns the number of friends the current user has.

**Parameters**

This method has no parameter

**Returns:**

Type: Number

Number of friends of the current user.

##requestFriend(username)

The method sends a friend request to the user.

**Parameters:**

• username

Type: String

Username of the user to sends the friend request to.

##post(statusUpdate)

The method posts a status update.

The status update can be up to 1000 characters long.

**Parameters:**

• statusUpdate

Type: String

Status update to post

**Returns:**

Type: Boolean

True if the post succeeded and false if the post fails.

##like(postId, likeType)

The method assigns the Likes to the specified post.

**Parameters:**

• postId

Type: Number

The ID number of the post to like

• likeType

Type: String

Valid values: &quot;Like&quot;, &quot;Love&quot;, &quot;Empathy&quot;

**Returns:**

Type: Boolean

True if the like succeeded and false if the like fails.