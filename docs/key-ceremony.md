# Key ceremony

Two people, one screen. Keys never touch a laptop that browses the web.

1. Generate session keys on the node, never on the workstation
2. Read the public key aloud, second person confirms each block
3. Submit `setKeys` from the node operator account
4. Record key and generation time in the ledger
5. `author_hasSessionKeys` must return true before the node rejoins

If the key is ever pasted into a chat, rotate it. Assume it leaked.
