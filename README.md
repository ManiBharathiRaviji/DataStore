# FreshWorks
DataStore:

This is the Backend Assignment given.

In this, I have used java to do some basic create,read and delete operations on a key-value 
data store which is stored in a text file.

# Create:
      A new key-value pair can be added to the data store using the Create operation. 
      The key is always a string - capped at 32chars. The value is always a JSON 
      object - capped at 16KB.  If Create is invoked for an existing key, an 
      appropriate error will be returned.

# Read:
      A Read operation on a key can be performed by providing the key, and receiving 
      the value in response, as a JSON object.

# Delete:
      A Delete operation can be performed by providing the key.
      
# Additional features:
      Every key supports setting a Time-To-Live property when it is created. This 
      property is optional.  If provided, it will be evaluated as an integer defining 
      the number of seconds the key must be retained in the data store. Once the 
      Time-To-Live for a key has expired, the key will no longer be available for 
      Read or Delete operations.Appropriate error responses will always be returned 
      to a client if it uses the data store in unexpected ways or breaches any limits. 
      The size of the file storing data will never exceed 1GB.
