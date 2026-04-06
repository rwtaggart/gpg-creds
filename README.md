# GPG Git Credentials Helper
`gpgcreds` uses the configured GPG signing key to store git credentials encrypted on disk.


## git credential helpers
The built-in credentials helper for git has two drawbacks:
1. It does not encrypt the passwords on disk. Credentials are only protected by filesystem access.
2. It does not support handling multiple accounts for the same remote host
3. I could not figure out how to work-around this with the following method. It never worked for me:
```sh
> git config --local credential.helper "store --file <separate-file>";
```

## REFERENCES
https://git-scm.com/docs/git-credential  
https://git-scm.com/doc/credential-helpers  
https://git-scm.com/docs/git-credential-store  
