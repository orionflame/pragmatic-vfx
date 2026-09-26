# Pragmatic Workflow website

Standalone product site for **Pragmatic Workflow**.

Public domain: https://workflow.pragmatic-vfx.com/

## Hosting

This repository is intended to publish from the repository root with GitHub Pages.

Custom domain:
```
workflow.pragmatic-vfx.com
```

DNS:
```
Type: CNAME
Name: workflow
Target: orionflame.github.io
```

For initial GitHub Pages certificate provisioning, use DNS-only at Cloudflare. After HTTPS is active, Cloudflare proxying can be evaluated separately.

## Publication checklist

1. GitHub repository Settings → Pages.
2. Publish from `master` / `(root)`.
3. Set custom domain to `workflow.pragmatic-vfx.com`.
4. In Cloudflare DNS, create the `workflow` CNAME pointing to `orionflame.github.io`.
5. Enable HTTPS in GitHub Pages after DNS validation succeeds.
6. Before commercial launch, replace the checkout URL tokens and supported-environment token in `index.html`.
7. Replace media placeholders through the slot configuration in `workflow.js`.

The main Pragmatic VFX website remains separate at https://pragmatic-vfx.com/.
