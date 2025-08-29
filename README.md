# Ventor Odoo Packages

This repository contains **4** Odoo packages from Ventor vendor.

## About Ventor

Ventor is a recognized vendor in the Odoo ecosystem, providing specialized addons and customizations.

## Packages Included (4 packages)

- **odoo-bringout-ventor-custom_import_wizard** - Custom Import Wizard
- **odoo-bringout-ventor-outgoing_routing** - Outgoing Routing
- **odoo-bringout-ventor-product_multiple_barcodes** - Product Multiple Barcodes
- **odoo-bringout-ventor-ventor_base** - Ventor Base


## Installation

Install any package from this collection:

```bash
# Install from local directory
pip install packages/ventor/PACKAGE_NAME/

# Install in development mode  
pip install -e packages/ventor/PACKAGE_NAME/

# Using uv (recommended for speed)
uv add packages/ventor/PACKAGE_NAME/
```

## Repository Structure

Each package in this repository follows the standard Odoo addon structure:

```
ventor/
├── odoo-bringout-ventor-ADDON/
│   ├── ADDON_NAME/           # Complete addon code
│   │   ├── __init__.py
│   │   ├── __manifest__.py
│   │   └── ... (models, views, etc.)
│   ├── pyproject.toml        # Python package configuration
│   └── README.md            # Package documentation
└── ...
```

## License

Each package maintains its original license as specified by Ventor.

## Support

For support with these packages, please refer to the original Ventor documentation or community resources.
