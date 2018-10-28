# Blockchain
Blockchain Transaction



Added the code for intialization of the envoirment,Each block doesn’t just contain the hash of the block before it, but its own hash is in part, calculated from the previous hash. If the previous block’s data is changed then the previous block’s hash will change ( since it is calculated in part, by the data) in turn affecting all the hashes of the blocks there after. Calculating and comparing the hashes allow us to see if a blockchain is invalid.



As you can see our basic Block contains a String hash that will hold our digital signature. The variable previousHash to hold the previous block’s hash andString data to hold our block data.
there are many cryptographic algorithms you can choose from, however SHA256 fits just fine for this example. We can import java.security.MessageDigest; to get access to the SHA256 algorithm.
We need to use SHA256 later down the line so lets create a handy helper method in a new StringUtil ‘utility’ class 
