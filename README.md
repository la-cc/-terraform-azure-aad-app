# Introduction:

The module is used to deploy azure over terraform with a default setup (Infrastructure as Code).

# Exmaple Use of Modul:

    module "aad_app" {
    source = "github.com/la-cc/terraform-azure-aad-app?ref=1.0.0"

    display_name                    = var.display_name
    redirect_uris                   = var.redirect_uris
    logout_url                      = var.logout_url
    app_owners                      = var.app_owners
    roles                           = var.roles
    app_role_assignment_required    = var.app_role_assignment_required

    }
