#[PeerGiving](www.peergiving.com)/less
PeerGiving is a fundraising platform that empowers charities and their fundraisers to succeed. 

To match the look and feel of a Peer Giving instance to a charity's brand, a front-end developer will need to reference code from this repository.

##Overview
The primary styling file for the un-themed Peer Giving platform is **css /** [**styles.less**](https://github.com/PeerGiving/less/blob/master/css/styles.less). This file pulls in all required styles for an unbranded PeerGiving product (including the Bootstrap framework).

The primary styling file for a given PeerGiving instance or *theme* is **[App_Themes](https://github.com/PeerGiving/less/tree/master/App_Themes) / [themeID] / styles.less**. This file pulls in:

1. the core styling file mentioned above
2. the **theme-variables.less** file (which is used to override core PeerGiving and Bootstrap variables)
3. the **theme.less** file (which is used for custom styling that is more complex than simple variable changes).

##Theme Variables

It is strongly recommended to copy from the template **App_Themes / _empty / [theme-variables.less](https://github.com/PeerGiving/less/tree/master/App_Themes/_empty/theme-variables.less)** when building a new theme from scratch.

You will find that variable values inherit up the following hierarchy tree:

1. bootstrap-3 / less / [variables.less](https://github.com/PeerGiving/less/blob/master/bootstrap-3.1.1/less/variables.less)
2. css / pgs / [variables.less](https://github.com/PeerGiving/less/blob/master/css/pgs/variables.less)
3. css / pgs / [theme-variables.less](https://github.com/PeerGiving/less/blob/master/css/pgs/theme-variables.less)
4. App_Themes / [themeID] / theme-variables.less
 
When overriding a variable, it's a good idea to trace it in order of inheritance.

##Finding where classes are used
At this time, we do not provide our HTML markup in this repository. Unfortunately that means you will not be able to search for all uses of a given style. 
