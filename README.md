# ZR CT Example Starter Recipe Installation Guide

To install the ZR CT Example Starter recipe, follow the steps below:

1. Ensure the below has been added to the `composer.json` **installer-paths**:
    ```sh
    "web/recipes/custom/{$name}": ["type:drupal-recipe"]
    ```
2. Run the following command:

    ```sh
    ddev drush recipe recipes/custom/zr-ct-example
    ```

3. Run the following command to install CKE5 configs:

    ```sh
    ddev drush cim --partial --source=recipes/custom/zr-cke5-recipe/config -y
    ```

This will complete the ZR CT Example Starter recipe installation.
