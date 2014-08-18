#[PeerGiving](www.peergiving.com)/less
PeerGiving is a fundraising platform that empowers charities and their fundraisers to succeed. 

To match the look and feel of a PeerGiving instance to a charity's brand, a front-end developer will need to reference code from this reposity.

##Overview
The primary styling file for the un-themed PeerGiving platform is **css /** [**styles.less**](https://github.com/PeerGivingSolutions/themes/blob/master/css/styles.less). This file pulls in all required styles for an unbranded PeerGiving product (including the Boostrap framework).

The primary styling file for a given PeerGiving instance or *theme* is **[App_Themes](https://github.com/PeerGivingSolutions/themes/tree/master/App_Themes) / [themeID] / styles.less**. This file pulls in:

1. the core styling file mentioned above
2. the **theme-variables.less** file (which is used to override core PeerGiving and Boostrap variables)
3. the **theme.less** file (which is used for custom styling that is more complex than simple variable changes).

It is strongly recommended to copy from the template **App_Themes / _empty / [theme-variables.less](https://github.com/PeerGivingSolutions/themes/tree/master/App_Themes/_empty/theme-variables.less)** when building a new theme from scratch.


