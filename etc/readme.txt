Product image sizes and other properties used on the storefront are configured in a view.xml configuration file. It is required for a theme, but is optional if exists in the parent theme.

If the product image sizes of your theme differ from those of the parent theme, or if your theme does not inherit from any theme, add view.xml using the following steps:

Log in to your Magento server as a user with permissions to create directories and files in the Magento installation directory. (Typically, this is the the Magento file system owner.)

Create the etc directory in your theme folder

Copy view.xml from the etc directory of an existing theme (for example, from the Blank theme) to your theme’s etc directory.

Configure all storefront product image sizes in view.xml. For example, you can make the category grid view product images square by specifying a size of 250 x 250 pixels, here is how the corresponding configuration would look like:

...
    <image id="category_page_grid" type="small_image">
        <width>250</width>
        <height>250</height>
    </image>
...
For details about images configuration in view.xml, see the Configure images properties for a theme topic.