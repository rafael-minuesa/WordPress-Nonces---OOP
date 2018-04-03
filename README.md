# WordPress-Nonces---OOP
Composer Package that implements WordPress Nonces as OOP

# WordPress Nonces

A nonce is a "number used once" to help protect URLs and forms from certain types of misuse, malicious or otherwise. WordPress nonces aren't numbers, but are a hash made up of numbers and letters. Nor are they used only once, but have a limited "lifetime" after which they expire. During that time period the same nonce will be generated for a given user in a given context. The nonce for that action will remain the same for that user until that nonce life cycle has completed.

WordPress's security tokens are called "nonces" despite the above noted differences from true nonces, because they serve much the same purpose as nonces do. They help protect against several types of attacks including CSRF, but do not protect against replay attacks because they aren't checked for one-time use. Nonces should never be relied on for authentication or authorization, access control. Protect your functions using current_user_can(), always assume Nonces can be compromised.
