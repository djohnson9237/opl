Notes
==========
The following are still in an early stage and need to be flushed out.

Updates to Works
-------------
How can the community talk about pros and cons of different versions?
Publish a new update as its own bit-torrent blob, but have meta-data point back 
to the original?

Server Architecture
-------------
If this gets popular, it will need to scale...how?

One (or more) hidden-service servers for content ratings. Just accept data from
clients, don't do any processing. That can happen on other computers, offline.
One (or more) hidden-service servers for user ratings. Just accept data from
clients, don't do any processing. That can happen offline.

Content submission system. Users can submit new works (or updates) that will 
then be listed for clients to download.

User registration service - accepts registrations from users and publishes 
public keys, hidden service addresses.

User Profile
-------------
When installing the client software, a public/private key pair is created for a
user. This will then be registered with a service. Any ratings of content or users will be signed with the user's private key before being submitted to the ratings
servers. When the batch processing happens on the ratings, the batch job will 
verify the signature by using the public key that the user registered with.

Rating Web of Trust
-------------
Rather than simply having the user ratings being determined by how many users 
rated that user, it would also be affected by their distance in the rating web
from the administrators of the server. This would prevent malicious users from
simply registering as many different users.
