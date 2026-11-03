# Disciplined Solo Stack

NetAnalyzers only. No Roslynator noise. 99% bugs caught as errors.

Why only NetAnalyzers?
- Built into .NET 8 SDK, no extra package needed for heaven
- One owner (【entity-Microsoft¦canonical_name=Microsoft】), one throat to choke
- Catches real crashes: null, dispose leak, SQL injection

What's inside?
- `Directory.Build.props` - perfect props that makes warnings = errors
- `.editorconfig` - only Security/Reliability/Usage as warning
- `.github/workflows/build.yml` - blocks PRs with bugs

How to use in PRoot Ubuntu:
dotnet build

If you see CS8600/CS8602 error, that's good. It just saved you from NullReference at 3am.

Built by a solopreneur in Las Pinas who was tired of community mess.
