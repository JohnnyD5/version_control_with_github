# How to re-authorize the OAuth Application 'Git Credential Manager'
**Error Message: git clone https://github.com/sede-x/Fluidization_FCC_Design_Tools.git
Cloning into 'Fluidization_FCC_Design_Tools'...
remote: The `sede-x' organization has enabled or enforced SAML SSO. To access
remote: this repository, you must re-authorize the OAuth Application `Git Credential Manager`.
fatal: unable to access 'https://github.com/sede-x/Fluidization_FCC_Design_Tools.git/': Failure when receiving data from the peer**

My company just enabled SSO for my Github Org overnight so was getting the same error running git pull. I fixed this with the following steps.

1. Open Credential Manager in Windows and delete the existing credential for github.com
2. Re-initialise the cred manager in git bash: git config --global credential.helper manager-core
3. Re-run git pull and follow the pop-up instructions to authenticate in a browser (which happened automatically for me with SSO).
4. After those steps git commands worked for me again.
