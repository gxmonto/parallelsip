# Security

## What is protected

- Every window runs sandboxed, with no remote content.
- SIP passwords are encrypted with the operating system's key store and are
  never written to the log.
- By default a line ignores SIP messages and call audio that do not come from
  its own server.
- Updates and speech models are downloaded over HTTPS and verified before use.
  Nothing installs during a call.

## What is not protected

- Call audio on the network is not encrypted (plain RTP). SIP signalling can
  use TLS.
- Transcripts and contacts are plain files in your user profile.
- Builds are not code-signed yet. Download only from the project's Releases
  page and check `SHA256SUMS.txt` if in doubt.

## Reporting

Open a private security advisory on the GitHub repository. Please do not file
public issues for security problems.
