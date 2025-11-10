# magento-aggregation

## Payfast Aggregation module v2.7.0 for Magento v2.4.8

This is the Payfast Aggregation module for Magento 2. Please feel free
to [contact the Payfast support team](https://payfast.io/contact/) should you require any assistance.

## Installation

1. **Download the Plugin**

    - **Option 1: Automatic Installation**
        - Install the module using the following composer command:
        ```console
        composer require payfast/payfast
        ```
    - **Option 2: Manual Installation**
        - Visit the [releases page](https://github.com/Payfast/magento-aggregation/releases) and
          download [Payfast.zip](https://github.com/Payfast/magento-aggregation/releases/download/v2.7.0/Payfast.zip).
        - Extract the contents of `Payfast.zip`, then upload the newly created **Payfast** directory into your Magento
          app/code directory (e.g. magentorootfolder/app/code/).
        - Run the following composer command:
         ```console
         composer require payfast/payfast-common:v1.4.0
         ```

2. **Install the Plugin**

    - Run the following Magento CLI commands:
      ```console
      php bin/magento module:enable Payfast_Payfast
      php bin/magento setup:upgrade
      php bin/magento setup:di:compile
      php bin/magento setup:static-content:deploy
      php bin/magento indexer:reindex
      php bin/magento cache:clean
      ```
3. **Configure the Plugin**

    - Login to the Magento admin panel.
    - Navigate to **Stores > Configuration > Sales > Payment Methods** and click on
      **Payfast**.
    - Configure the module according to your needs, then click the **Save Config** button.
    - Navigate to **Stores**, and add **ZAR** under Currency Symbols and Rates.

Please [click here](https://payfast.io/integration/plugins/magento/) for more information concerning this
module.

## Collaboration

Please submit pull requests with any tweaks, features or fixes you would like to share.





