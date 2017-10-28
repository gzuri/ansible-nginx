# Overview
Repository contains an ansible script that sets up website on nginx. 
Website is protected using let's encrypt certificate, with the default redirect to https.

# Usage
```
ansible-playbook -s --ask-sudo-pass --extra-vars "domain={domain} letsencrypt_email={email for renewals}" nginx.yml
```

# Motivation
Setting up websites is a repetetive task that can be easly automated. 