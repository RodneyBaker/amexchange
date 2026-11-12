# URLs and resource information

Animation:Master resources have a URL field. Use it to point to useful,
maintained information about the resource, while keeping the resource usable
when that destination is unavailable.

## Choose the destination

- Link to the creator's project page, discussion, or other authoritative
  external page when one exists and is useful to users.
- For information that must travel with the exchange copy, add an `info.html`
  file beside the resource and set the resource URL to that file. Include the
  creator, usage notes, license, credits, and any associated files there as
  relevant. Keep the page self-contained or use relative links to files shipped
  with the resource; do not link to paths on the contributor's computer.
- If several resources share a catalog page, they may point to that page with
  a distinct fragment or documented anchor for each resource. Keep the
  resource name visible in the page so the destination remains understandable
  if the application or browser drops the fragment.
- A dedicated single-file TiddlyWiki can serve as a shared catalog when it is
  distributed with the resources and works offline. Document how to open it
  and use stable, human-readable tiddler names in links.

## Keep links portable

Use a URL that works for someone opening the resource from the exchange, not
one that only works on the contributor's machine. Check relative links from a
copied resource folder and avoid requiring network access for essential usage
instructions or files. Do not change a user's global URL preference as part of
contributing a resource.

Animation:Master also has an installation-level `Support.html` used by its
Community window. That application support page is separate from this exchange
and may not be installed in the same location for every user. Resources should
not assume it is present or use it as their only documentation destination.
