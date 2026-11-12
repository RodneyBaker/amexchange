# Images in shared resources

Keep the exchange focused on editable Animation:Master resources. An image is
included only when it helps someone identify a resource or is needed to use or
rebuild it.

## Resource previews

- Prefer Animation:Master's existing preview data when the preview only needs
  to appear in Animation:Master. This uses the format's current support and
  avoids adding another file to the exchange.
- When a preview needs to be visible outside Animation:Master, include one
  optional PNG or JPEG beside the resource, using the same base name (for
  example, `CoolModel.mdl` and `CoolModel.png`). Keep it a compact thumbnail;
  do not include multiple sizes or a full-resolution render as a preview.
- Do not embed base64 images in `.mdl` files. The format and tools in this
  repository do not provide a documented way to create or consume them, and
  embedding would increase file size and require format/tooling changes.
- SVG is not a supported preview format for the current Animation:Master
  workflow. Convert a preview to PNG or JPEG when a sidecar is needed.

## Images required by a resource

If a model or project needs an image (such as a decal or texture), include the
image with the resource and preserve any relative paths expected by the
project. Use clear filenames and common formats supported by Animation:Master.
Do not rely on a file from an author's machine or on a remote URL.

When an image can be regenerated from included project data, include that
editable source data and explain how to regenerate the image in the resource's
own `readme` file. Include the generated image too if it is needed to open or
use the resource as shared. This keeps the resource useful while allowing
others to edit and rebuild it.

## Keep the exchange lightweight

Before adding an image, check whether the existing preview or project data is
enough. Crop previews to their subject, remove unused layers and metadata, and
avoid duplicate or unnecessarily large images. Do not impose a fixed byte
limit: required textures and project images vary, so describe unusually large
assets and why they are needed in the resource's documentation.
