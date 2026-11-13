# Read-Only Source Investigation

Read this reference when the user asks to authenticate or trace a specific message, sender, list, domain, or provider.

## Collect evidence safely

- Prefer already cached raw source or headers obtained through a method known not to render the body, fetch remote content, alter selection, or change local/server flags.
- If that is unavailable, ask for raw source or report the limitation. Do not open a message and then mark it unread as a substitute.
- Treat display names, `From`, `Reply-To`, body links, and advertised unsubscribe destinations as claims, not identity proof.

## Correlate the source

Use the trusted receiver's `Authentication-Results` as the starting point. Correlate its SPF, DKIM, and DMARC assessments with `DKIM-Signature`, the trusted `Received` chain, `Return-Path`, `Message-ID`, `List-Unsubscribe`, and `List-Unsubscribe-Post`. Distinguish:

- authenticated/aligned sending domain;
- visible author or promoted brand;
- envelope sender and reply infrastructure;
- originating or relaying IP/provider; and
- linked landing, tracking, or unsubscribe infrastructure.

A generic SPF/DKIM pass or a reputable relay does not by itself authenticate the visible organization or a list-unsubscribe destination.

## Verify infrastructure

Use current official RDAP/registry, ASN or host, registrar, provider, and abuse-contact sources. Navigate independently; never visit body links or personalized unsubscribe URLs to identify infrastructure. Deduplicate exact messages and group by stable authenticated domain, list ID, or delivery account.

## Report evidence levels

Separate verified header evidence, official infrastructure records, provisional correlations, and unresolved claims. Report the minimum useful identifiers and do not expose recipient addresses, full headers, or personalized tokens unless the user authorizes a necessary disclosure.

Read-only investigation ends with findings. It never authorizes an unsubscribe, complaint, reply, provider report, or other external action.
