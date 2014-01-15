Amendments
==========

Once a PSR has been "Accepted", the PSR meaning cannot change, backwards 
compatibility will remain at 100%, and any confusion that arises from original 
wording may only be clarified through Errata - as outlined in 
`bylaws/004-psr-workflow.md`.

If a PSR is found to require updates or errata is no longer serves as a 
useful resource to clarify confusion, then the PSR must be replaced, following
the workflow set out in `bylaws/004-psr-workflow.md`.

The original PSR may then be deprecated, and the new PSR becomes the recommended 
document. 

## 1. Dependencies 

As documents are expected to be replaced rather than amended, dependencies on 
other PSR's should be avoided whenever possbible. For instance, the follow is 
no longer permitted:

> - Namespaces and classes MUST follow PSR-0.

Instead the following example must be used:

> - Namespaces and classes MUST follow an autoloading PSR: [PSR-0].

These square brackets denote a "reference area", which is a list of PSRs that
conform to the rule. These may ONLY be added to, and never removed.

> - Namespaces and classes MUST follow an autoloading PSR: [PSR-0, PSR-4].

As new PSRs are created which satisfy a requirement, they may be added. Even if 
adding a new PSR involves deprecating another PSR, that deprecated PSR will 
remain in the document, as anything else would break backwards compatibility.

## 2. Acceptable Amendments

Other than the updating of dependency references, there are two other potentialy 
acceptable amendment scenarios. 

### 1. Deprecation and Replacement

A vote has been won with the decision to deprecate a PSR and superceed it 
with another PSR. The deprecated PSR must be marked as such in the original 
document, and a link should be placed in the body.

For example:

> **Deprecated** - As of 01/01/2014 PSR-0 has been marked as deprecated. PSR-4 is now recommended 
as an alternative.

### 2. Annotations

If Errata is added which is deemed important enough, annotations may be placed in 
or near the offending line so that readers know to view the errata for more 
information.

> - Something confusing about where brackets go. [cf. [errata](foo-meta.md#anchor)]

### 3. Formatting & Typos

If formatting is broken for any reason (due to GitHub Markdown issues) then 
changing formatting must not be considered a change to the document.
