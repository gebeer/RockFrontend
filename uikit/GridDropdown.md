# GridDropdown UIkit Component

Note that nested grids are not supported!

## Usage

Just add the `rf-griddropdown` class to the grid where you want to use the dropdowns. Then add the `rf-griddropdown-toggle` to the element that toggles the dropdown and then add a hidden element directly after the toggle. This is the markup that will be used to populate the dropdown!

```html
<div class='rf-griddropdown' uk-grid>
  {foreach $items as $item}
    <div class='uk-width-1-3'>
      items visible content
      <a class='rf-griddropdown-toggle'>show info</a>
      <div class='uk-hidden'>
        <button class="uk-alert-close" type="button" uk-close></button>
        your dropdown markup here
      </div>
    </div>
  {/foreach}
</div>
```