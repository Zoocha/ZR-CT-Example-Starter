# ZR CT Example Starter Recipe Installation Guide

To install the ZR CT Example Starter recipe, follow the steps below:

1. Open your terminal.
2. Navigate to your project directory. 
3. Add the below in the Drupal Root's composer.json installer-paths
```sh
"web/recipes/custom/{$name}": ["type:drupal-recipe"]
```
4. Run the following command:

    ```sh
    ddev drush recipe recipes/custom/zr-ct-example
    ```
5. Run the below command to install CKE5 configs
    ```sh
    ddev drush cim --partial --source=recipes/custom/cke5-recipe/config -y
    ```
This command will execute the ZR CT Example Starter recipe installation.
