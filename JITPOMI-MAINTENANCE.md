# Maintained compatibility branch

Base: upstream `v0.8.2`. All upstream source, history and licenses are retained.

Replace paste with maintained pastey. Preserve exported macro names and wire format. Update the rtnetlink example to current route APIs and test it against this core implementation.

This is an explicit JITPOMI-maintained source branch, not a claim that upstream released this change. Applications must pin the reviewed commit. No advisory ignores, renamed copies of the obsolete dependencies, TLS bypasses or target filters are used.

Validation: `cargo test --all-targets && cargo test --doc` plus DogRS/Business integration and audit checks. On upstream release, verify the source/API and stored-format compatibility, rerun the same checks, and replace the source pin with the maintained registry release.
