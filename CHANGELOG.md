# v4.1.0
- Added more comments to the layout templates
- Added `.text-overflow()` and `.transition()` mixins to the stylesheet
- Added better dialog styles to the stylesheet
- Added a font-size for the `.note` typography class
- Added better styles to the Password-protected Board template
- Removed Flexbox mixins from the stylesheet now that Flex has better browser support
- Removed navigation tree dropdown links from the stylesheet because they're bad and I hate them (set `.popup_html` to `display: none`)
- Removed the div selectors from title bar controls
- Removed the div selectors from pagination
- Removed the erroneous table cell border from the Post List and Message List templates
- Removed line height from the WYSIWYG submit button (let it take the default button line height)
- Moved some variables around for better organization
- Updated heading font sizes
- Updated `@timestamp`, `@description`, `@viewing`, and `@small` variables to inherit rather than have their own styles
- Updated `@link_font` variable to inherit rather than have its own styles
- Updated `font-weight: bold` properties to use the `@bold_weight` variable for consistency
- Updated the icon selector in title bar controls
- Updated the class name for the footer link wrapper (was `.c-footer__links` now `.c-footer__link-wrapper`)
- Updated the heights of ad wrappers
- Messed around with the Search Page template

# v4.0.0
- So many changes...

# v2.0.6
- Corrected the issue where clicking pagination links causes Font Awesome icons to disappear

# v2.0.5
- Hooked up the Board icons to the correct variables (previously they were all using the same variable)

# v2.0.4
## Visual Editor
- Added objects for Thread icons, Conversation icons
- Added object for `.container` links hover color
- Added object for Info Center links hover color
- Added object for Conversation subject alignment

## Navigation
- Moved Navigation tip holder back inside of Navigation item anchor

## Icons
- Replaced Thread and Conversation icons with Font Awesome icons

## Pagination
- Added script to remove left and right double angle quotes from pagination

## Shoutbox
- Added `10px` padding to `.shoutbox.container > .content` to correct a padding issue

# v2.0.3
## Visual Editor
- Added objects for Board icons, checkmark icon

## Icons
- Replaced Poll checkmark icon with Font Awesome icon

## User Profile
- Added more padding to the User Avatar with `.pad-right-double` instead of `.pad-right`
- Added `.groups_title` class to table headers for the Groups tab
- Styled `.groups_title` with `text-align: center` and `padding-left: 20px` to line it up with the Group names row below

# v2.0.2
## Images
- Added Smangii's ClearUBBC icons

## Visual Editor
- Removed `text-shadow` objects
- Removed `border-radius` objects
- Added objects for Footer text
- Added objects for Forum Wrapper images
- Added objects for Sidebar
- Added objects for "Like", "Settings", "Search", "Locked", "Bookmark", and "Poll" font icon colors

## Base
- Reorganized stylesheet with more descriptive comment headers
- Moved styles to more logical sections to make them easier to find
- Removed rounded corners, box-shadow mixins + all references in CSS
- Added predefined Sidebar styles with variables
- Added predefined Forum Wrapper styles with variables
- Styled `body` with `line-height: 1.4` to fix descenders on text being cut off
- Added mixin `.fixed-navigation` for easy sticky top nav
- Added Font Awesome icons

## Global Variables
- Set `@body_background_image` to `@empty` so that it can be predefined elsewhere without causing an error
- Set `@default_forum_text_font_size` to `13px` instead of `10pt`
- Set `@default_forum_text_font_family` to the Google Font "Open Sans"
- Set `@default_forum_text_decoration`, `@default_forum_text_case`, and `@default_forum_text_caps` to `@empty`
- Set `@link_hover_color` to `lighten(@link _color, 20%)`
- Added `@container_links_hover_color` with default `@link_hover_color` to create a consistent link hover color

## Ads
- Added section for Ad styles
- Added `#top-ad-banner { margin: 20px auto !important; }`
- Added `#bottom-ad-banner { margin: 10px auto !important; }`

## Header
- Removed `text-shadow` from `a#logo`
- Set `@banner_text_font` to `@default_forum_text_font_family` to be consistent

## Navigation
- Removed `@nav_bar_button_shadow` + all references in CSS
- Removed `@welcome_text_shadow` + all references in CSS
- Set `@nav_bar_button_font` to `100% @default_forum_text_font_family` to be consistent
- Set `@nav_bar_bubble_font` to `80% @default_forum_text_font_family` to be consistent
- Set `@welcome_text_font` to `100% @default_forum_text_font_family` to be consistent
- Moved Navigation tip holder outside of Navigation item anchor to make it easier to style when inline with the parent Navigation item
- Styled `#navigation-menu > ul li` with `position: relative` to contain tip holder
- Styled `#navigation-menu div.tip-holder` with `cursor: pointer` to show it is clickable
- Removed unused span wrapping `Welcome $[current_user.name]` in Forum Wrapper layout template

## Navigation Tree
- Set `@nav_tree_font` to `80% @default_forum_text_font_family` to be consistent
- Reduced padding on `#nav-tree > li a` to `3px 10px 3px 15px` to vertically align nav item text
- Styled `.recent-threads-button .new-icon` with `margin: 1px 5px 0 0` to line it up with "Participated"

## Forum Wrapper
- Set `@wrapper_bottom_margin` to `20px` to adjust for space between `#wrapper` and `#footer`

## News
- Styled `#news` with `height: 20px !important` to make it the same height as Navigation Tree
- Added `#news .items .itemSlide { line-height: 20px !important; }` to make it the same height as Navigation Tree
- Styled `#news .nav > span.title` with `height: 20px !important` to make it the same height as Navigation Tree

## Info Center
- Added `@info_links_hover_color: @container_links_hover_color`
- Set `@info_links_decoration` to `@link_hover_decoration` to be consistent
- Set `@info_titles_font` to `@info_text_font` to be consistent
- Rebuilt Info Center to have fewer nested tables
- Fixed resulting double border styles
- Removed `.small span` wrapping timestamp in "Members" cell to make it the same size as the timestamp in "Threads & Posts" cell

## Footer
- Moved `$[footer]` outside of `#wrapper` so Ads and Footer content don't disrupt the inner spacing of the Forum Wrapper if it has a bg color/image
- Gave `$[footer]` parent div of `#footer` so that it can be centered and spaced more easily
- Set `@footer_text_font` to `@default_forum_text_font_family` to be consistent
- Added `@footer_width`
- Set `@footer_width` to `width: @wrapper_width` to be the same width as the Forum Wrapper
- Styled `#footer` with `margin: 0 @wrapper_right_margin @wrapper_bottom_margin @wrapper_left_margin` to line up with the Forum Wrapper
- Styled `#footer` with `@footer_text_font` to be consistent
- Removed padding from Footer
- Added `@footer_link_color`, `@footer_link_font`, `@footer_link_decoration`
- Set `@footer_link_color` to `@link_color`
- Set `@footer_link_font` to `100% @footer_text_font`
- Set `@footer_link_decoration` to `@link_decoration`
- Set `@footer_hover_color` to `@link_hover_color`
- Set `@footer_hover_font` to `@footer_link_font`
- Set `@footer_hover_decoration` to `@link_hover_decoration`

## Pages
- Set `.search .content form > div` to `margin: 10px` rather than just a right and bottom margin

## Titles
- Kept `@title_text_shadow` + all references in CSS because it's useful

## Containers
- Added `.container:last-of-type { margin-bottom: 0; }` so that last `.container` doesn't add extra space to `#wrapper` if it has a bg color/image
- Added `.content-box a:hover, .container a:hover` with `color: @container_links_hover_color` to make consistent hover colors

## Buttons
- Set `@buttons_background_image` to `@empty`
- Set `@buttons_background_repeat` to `@empty`
- Set `@buttons_border`, `@buttons_hover_border`, and `@buttons_active_border` `border-color` to `@container_inner_border_color`
- Set `@buttons_text_font` to `13px @default_forum_text_font_family` to be consistent
- Set `@buttons_hover_background` to `@empty`
- Set `@buttons_hover_text_color` and `@buttons_active_text_color` to `@buttons_text_color`
- Added `.button { background-image: none; -webkit-border-radius: 0; border-radius: 0; }`

## Icons
- Styled `.new-icon, .new-icon a` with `line-height: 9px !important; height: 9px;`
- Styled `.new-icon` with `padding: 0 2px;`
- Replaced "Like", "Settings", "Search", "Locked", "Bookmark", "Poll", and Board icons with Font Awesome icons
- Styled `a.likes-button` with `padding: 3px 7px 1px; font-size: 12px`
- Styled `.button .status` with `padding: 0 8px 0 8px`
- Removed `margin-left` from `.ui-search .search-filters-button`
- Styled `.ui-search .search-filters-button` with `padding: 2px 7px 3px`
- Styled `.posts .poll_icon` with `padding-right: 7px`
- Styled `.posts .bookmark_icon` with `padding-right: 9px`

## Dialogs
- Removed `border-radius` from `.ui-selectMenu-box`
- Added `.ui-widget-overlay { opacity: 0.3; }` under dialogs to darken the background overlay on modal windows
- Added script to allow background overlay on modal windows to be darkened

## Pagination
- Set `.ui-pagination li > a, .ui-pagination li > div` `border-color` to `@container_inner_border_color`
- Set `.ui-pagination li > a:hover, .ui-pagination li > div:hover` `border-color` to `@pagination_hover_color`
- Set `.ui-pagination li.state-disabled > a:hover` `border-color` to `@pagination_background_color`

## Tables/Lists/Forms
- Set `@lists_hover_links_decoration` to `none`
- Set `@lists_hover_links_color` to `@container_links_hover_color` to make consistent hover colors

## User Profile
- Styled `.show-user #right-column` with `width: 132px` to create consistent content padding
- Styled `.show-user .right-col` with `width: 120px; padding: 8px 10px; .box-sizing();` to create consistent content padding
- Styled `.show-user .list .main` with `padding: 5px 20px` and `.show-user .time-container` with `5px 20px 5px 0` to create consistent content padding
- Styled `.show-user .notifications .main` with `padding: 10px 20px` to create consistent content padding
- Made padding consistent on first tab with `.pad-all-thick` instead of `.pad-all-double`

## Board List
- Set `@board_names_font` `font-size` to `100%`
- Set `@board_mod_font` to `80% @default_forum_text_font_family` to be consistent
- Set `@board_sub_font` to `80% @default_forum_text_font_family` to be consistent
- Set `.boards .main` width to `auto`
- Removed `@board_align_posts`
- Changed `@board_align_threads` to `@board_align_count`
- Made `.boards .threads` and `.boards .posts` same width
- Styled `.boards .threads` and `.boards .posts` with `text-align: @board_align_count`
- Moved `by $[board.last_thread.last_post.created_by]` next to recent post link rather than under it on Board List layout template
- Changed `.description`, `.moderators`, and `.sub-boards` on Board List layout from paragraph tags to div tags
- Removed Legend and Stats table
- Removed "Board, Threads, Posts, Last Post" row from Board List layout template
- Added "Threads" and "Posts" label under associated numbers to Board List layout template

## Post List
- Added script to remove default inline styles from the Thread Description plugin because they were `!important` and could not be overwritten through the stylesheet
- Appended `.thread_description_page` to `.messages .participants` CSS rule to make them the same
- Fixed padding on `.control-bar` items
- Styled `.posts span.labels` with `padding: 0 6px 4px 6px` to adjust spacing between borders

## Messages List
- Styled `.messages .item > td` with `border-width: 0` to remove extra inner 1px border on far right in Message List layout template
- Set `.messages .participants` to only have bottom border
- Added `.last` to `<th class="latest">` to remove extra inner 1px border on far right in Conversations Page layout template
- Styled `.conversations .main` with `text-align: @conversation_align_subject` to make it consistent with the Thread List
