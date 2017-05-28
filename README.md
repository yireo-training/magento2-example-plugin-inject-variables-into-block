# Example Block interceptor
Example Magento 2 module showing how to use an interceptor to extend Block classes

## Installation
To install use the following composer command:

    composer require yireo-training/magento2-example-plugin-inject-variables-into-block

Next enable the module:

    bin/magento module:enable Yireo_ExamplePluginInjectVariablesIntoBlocks
    bin/magento setup:upgrade
    
And flush the cache:

    bin/magento cache:clean

# Proof of concept
The block with XML layout name `absolute_footer` should be replaced with a new PHTML template that also
includes an `$customer` variable.
