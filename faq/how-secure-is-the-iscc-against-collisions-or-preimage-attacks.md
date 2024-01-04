# How secure is the ISCC against collisions or preimage attacks?

The ISCC uses a Blake3 hash as a 256-bit MultiHash for the Instance-Code. Blake 3 is considered to be a very secure and fast hashing algorithm, which is used in a wide range of crypto applications and contexts, such as IPFS. It is designed to be very secure against collisions, preimage, and other types of attacks.

Blake3 is considered to be collision-free up to a number of 2^64 possible hashes, being a very large number and resulting in an extremely low probability of hash collisions.

2^64 is approximately 18.4 quintillion. One quintillion has 18 zeros: 1,000,000,000,000,000,000 in numerical form. To put this number in perspective, consider that the estimated number of grains of sand on all the beaches on Earth is around 7.5 quintillion.

A preimage attack, also known as an “inversion attack,” is a type of cryptographic attack that attempts to derive the input (or “preimage”) from a specific output when processed by a cryptographic hash function. Blake3 is very resistant to preimage attacks.

The first three units of the ISCC, the Meta-Code, the Content-Code, and the Data-Code, are similarity preserving hashes, which means that they are not cryptographic hashes and not designed to be resistant to collisions.

SimHash is a locality-sensitive hash function, which means that it is designed to produce similar outputs for similar inputs. This is useful for identifying duplicate or near-duplicate content, which can be useful for detecting plagiarism or for finding duplicate web pages. The main idea behind SimHash is to convert the input data into a fixed-length bit string in such a way that similar inputs will have similar output hashes. This is done by converting the input data into a set of numerical feature values, and then combining the values received into a single hash value using a technique called “feature hashing.”

IMPORTANT NOTE: It is considered insecure, and it is not recommended to create and publish hashes of any sort generated from documents such as forms, as many forms contain sensitive information, e.g., personal identifiable information (PII), IDs like social security numbers, or financial information. If the hash of one form is exposed, it might be possible for an attacker to access this information.
