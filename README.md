# cURLcraft

Just like with the wget wizard, but for cURL and still offline. The HTML file is all that you need.

You can do fun and exciting things for choosing options and get a ready-to-run `curl` command that updates as you go. The options are:
- Request: URL(s), method, custom method and headers.
- Body: JSON, raw text, URL-encoded form fields, multipart with file uploads, binary file or `PUT` upload.
- Authentication and identity: basic, digest, bearer, API-key header or `.netrc.` This section also has cookies, user agent and referrer.
- Behavior: redirects, compression, HTTP version, fail-on-error and globbing.
- TLS, proxy and network: certificate options, proxy, host override and IP version.
- Timeouts and retries: timeouts, retries, resume and speed limit.
- Output and display: where the response goes, headers, verbosity and `--write-out` stats such as a timing breakdown.

Beyond the Wget Wizard like UI, I added a few more things:

- Explanation panel: it breaks the command into parts and says what each one does.

- Quick-start recipes: examples such as POST JSON, a resumable download, a timing check and a cookie login.

- Shell and syntax choices: bash/zsh, PowerShell or cmd, with the right quoting, `curl.exe` on Windows, and short or long flags.

- Warnings: for invalid JSON, secrets that would land in shell history, a missing URL scheme and shell-specific quoting problems.

Windows PowerShell 5.1 strips double quotes from arguments passed to `curl.exe`, so JSON bodies break there. The page warns about this and suggests PowerShell 7 or putting the body in a file. Minify JSON is on by default, so the body goes on one line.

<img width="774" height="968" alt="curl1" src="https://github.com/user-attachments/assets/a8ec7f01-0f12-4f10-9ed7-a758b7b77435" />
