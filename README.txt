RYUMA iOS DYLIB - recovered source project

License behavior in this new DYLIB:
- Embedded key: RYUMA-iOS-SR1FF
- Verification endpoint: https://ryuma-verify.ieuhehhehehehhrh.workers.dev
- The key is sent automatically to the Worker as POST JSON: {"key":"RYUMA-iOS-SR1FF"}.
- The login screen displays the embedded key as read-only and starts verification automatically.
- The Worker remains authoritative: a successful HTTP 200 response with {"valid":true} is accepted.

This is source code and a GitHub Actions workflow, not a compiled or tested DYLIB.
Build on GitHub Actions and verify the workflow succeeds before installing.
The embedded key can be extracted from a client-side DYLIB; this is not a secret-storage mechanism.
The old DYLIB and its key/server are not included or modified by this project.
