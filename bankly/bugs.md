- First Bug:
	- Changed jwt.decode(token) --> jwt.verify(token)
	- jwt.decode(token) = decodes signed JWTs without validating the signatures on the token
	
- Second Bug:
	- User.authenticate was missing await.
	- Added await

- Third Bug:
	- User.delete missing await
	- Added await