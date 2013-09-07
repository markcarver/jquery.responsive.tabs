jQuery Responsive Tabs
======================

Here is an example of how to make various Drupal tabs responsive:
```js
/**
 * Responsive Tabs
 */
if ($.fn.responsiveTabs) {
  Drupal.behaviors.responsiveTabs = {
    attach: function(context) {
      // Make tabs responsive.
      $('ul.nav-tabs, ul.tabs.primary, ul.tabs.secondary, ul.quicktabs-tabs, ul.horizontal-tabs-list', context).responsiveTabs({
        activeClass: 'active',
        activeSelectors: '.active, .selected, .active-trail',
        icon: '<i aria-hidden="true" class="icon fontello icon-down-open"></i>',
        text: 'more tabs'
      });
    }
  };
}
```
