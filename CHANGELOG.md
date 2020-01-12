### v4.0.0
- So many changes...

### v2.0.6
- Corrected the issue where clicking pagination links causes the Font Awesome glyphs to disappear

### v2.0.5
- Hooked up the board icons to the correct variables (previously they were all using the same variable)

### v2.0.4
visual editor ---
- Added objects for thread icons, conversation icons
- Added object for container links hover color
- Added object for info links hover color
- Added object for conversation subject alignment

navigation ---
- Moved navigation tip holder back inside of navigation item anchor

icons ---
- Replaced thread, conversation icons with Font Awesome glyphs

pagination ---
- Added script to remove left and right double angle quotes from Prev/Next

shoutbox ---
- Added 10px padding to .shoutbox.container > .content to correct padding issue

### v2.0.3
visual editor ---
- Added objects for board icons, checkmark icon

icons ---
- Replaced poll checkmark icon with Font Awesome glyph

profile ---
- Added more padding to the user avatar with .pad-right-double instead of .pad-right
- Added .groups_title class to table headers for Groups tab
- Styled .groups_title with text-align: center and padding-left: 20px to line it up with group names row below

### v2.0.2
images ---
- Added Smangii's ClearUBBC icons

visual editor ---
- Removed text shadow objects
- Removed border radius objects
- Added objects for footer text
- Added objects for wrapper images
- Added objects for sidebar
- Added objects for "like", "settings", "search", "locked", "bookmark", and "poll" font glyph colors

base ---
- Reorganized stylesheet with more descriptive comment headers
- Moved styles to more logical sections to make them easier to find
- Removed rounded corners, box shadow mixins + all references in CSS
- Added predefined sidebar styles with variables
- Added predefined wrapper styles with variables
- Styled body with line-height: 1.4 to fix descenders on text being cut off
- Added mixin .fixed-navigation for easy sticky top nav
- Added Font Awesome

global variables ---
- Set @body_background_image to @empty so that it can be predefined elsewhere without causing an error
- Set @default_forum_text_font_size to 13px instead of 10pt
- Set @default_forum_text_font_family to Google Font "Open Sans"
- Set @default_forum_text_decoration, @default_forum_text_case, and @default_forum_text_caps to @empty
- Set @link _hover_color to lighten(@link _color, 20%)
- Added @container_links_hover_color with default @link _hover_color to create a consistent link hover color

ads ---
- Added section for ad styles
- Added #top-ad-banner { margin: 20px auto !important; }
- Added #bottom-ad-banner { margin: 10px auto !important; }

header ---
- Removed text-shadow from a#logo
- Set @banner_text_font to @default_forum_text_font_family to be consistent

navigation ---
- Removed @nav_bar_button_shadow + all references in CSS
- Removed @welcome _text_shadow + all references in CSS
- Set @nav_bar_button_font to 100% @default_forum_text_font_family to be consistent
- Set @nav_bar_bubble_font to 80% @default_forum_text_font_family to be consistent
- Set @welcome _text_font to 100% @default_forum_text_font_family to be consistent
- Moved navigation tip holder outside of navigation item anchor to make it easier to style when inline with the parent navigation item
- Styled #navigation-menu > ul li with position: relative to container tip holder
- Styled #navigation-menu div.tip-holder with cursor: pointer to show it is clickable
- Removed unused span wrapping "Welcome $[current_user.name]." in Forum Wrapper layout template

nav tree ---
- Set @nav_tree_font to 80% @default_forum_text_font_family to be consistent
- Reduced padding on #nav-tree > li a to 3px 10px 3px 15px to vertically align nav item text
- Styled .recent-threads-button .new-icon with margin: 1px 5px 0px 0px to line it up with "Participated"

wrapper ---
- Set @wrapper_bottom_margin to 20px to adjust for space between #wrapper and #footer

news ---
- Styled #news with height: 20px !important to make it the same height as nav tree
- Added #news .items .itemSlide { line-height: 20px !important; } to make it the same height as nav tree
- Styled #news .nav > span.title with height: 20px !important to make it the same height as nav tree

info center ---
- Added @info_links_hover_color: @container_links_hover_color
- Set @info_links_decoration to @link _hover_decoration to be consistent
- Set @info_titles_font to @info_text_font to be consistent
- Rebuilt info center to have less nested tables
- Fixed resulting double info center border styles
- Removed .small span wrapping timestamp in members cell to make it the same size as the timestamp in threads &amp; post cell

footer ---
- Moved $[footer] outside of #wrapper so ads and footer content don't disrupt the inner spacing of the wrapper if it has a bg color/image
- Gave $[footer] parent div of #footer so that it can be centered and spaced more easily
- Set @footer_text_font to @default_forum_text_font_family to be consistent
- Added @footer_width
- Set @footer_width to width: @wrapper_width to be the same width as forum wrapper
- Styled #footer with margin: 0 @wrapper_right_margin @wrapper_bottom_margin @wrapper_left_margin to line up with forum wrapper
- Styled #footer with @footer_text_font to be consistent
- Removed padding from footer
- Added @footer_link_color, @footer_link_font, @footer_link_decoration
- Set @footer_link_color to @link _color
- Set @footer_link_font to 100% @footer_text_font
- Set @footer_link_decoration to @link _decoration
- Set @footer_hover_color to @link _hover_color
- Set @footer_hover_font to @footer_link_font
- Set @footer_hover_decoration to @link _hover_decoration

pages ---
- Set .search .content form > div to margin: 10px rather than just a right and bottom margin

titles ---
- Kept @title_text_shadow + all references in CSS because it's useful

containers ---
- Added .container:last-of-type { margin-bottom: 0; } so that last .container doesn't add extra space to #wrapper if it has a bg color/image
- Added .content-box a:hover, .container a:hover with color: @container_links_hover_color to make consistent hover colors

buttons ---
- Set @buttons_background_image to @empty
- Set @buttons_background_repeat to @empty
- Set @buttons_border, @buttons_hover_border, and @buttons_active_border border-color to @container_inner_border_color
- Set @buttons_text_font to 13px @default_forum_text_font_family to be consistent
- Set @buttons_hover_background to @empty
- Set @buttons_hover_text_color and @buttons_active_text_color to @buttons_text_color
- Added .button { background-image: none; -webkit-border-radius: 0; border-radius: 0; }

icons ---
- Styled .new-icon, .new-icon a with line-height: 9px !important; height: 9px;
- Styled .new-icon with padding: 0px 2px;
- Replaced "like", "settings", "search", "locked", "bookmark", "poll", and board icons with Font Awesome glyphs
- Styled a.likes-button with padding: 3px 7px 1px; font-size: 12px
- Styled .button .status with padding: 0px 8px 0px 8px
- Removed margin-left from .ui-search .search-filters-button
- Styled .ui-search .search-filters-button with padding: 2px 7px 3px
- Styled .posts .poll_icon with padding-right: 7px
- Styled .posts .bookmark_icon with padding-right: 9px

dialogs ---
- Removed border-radius from .ui-selectMenu-box
- Added .ui-widget-overlay { opacity: .3; } under dialogs to darken the background overlay on modal windows
- Added script to allow background overlay on modal windows to be darkened

pagination ---
- Set .ui-pagination li > a, .ui-pagination li > div border-color to @container_inner_border_color
- Set .ui-pagination li > a:hover, .ui-pagination li > div:hover border-color to @pagination_hover_color
- Set .ui-pagination li.state-disabled > a:hover border-color to @pagination_background_color

tables/lists/forms ---
- Set @lists_hover_links_decoration to none
- Set @lists_hover_links_color to @container_links_hover_color to make consistent hover colors

profile ---
- Styled .show-user #right-column with width: 132px to create consistent content padding
- Styled .show-user .right-col width width: 120px; padding: 8px 10px; .box-sizing(); to create consistent content padding
- Styled .show-user .list .main with padding: 5px 20px and .show-user .time-container with 5px 20px 5px 0 to create consistent content padding
- Styled .show-user .notifications .main with padding: 10px 20px to create consistent content padding
- Made padding consistent on first tab with .pad-all-thick instead of .pad-all-double

board list ---
- Set @board_names_font font-size to 100%
- Set @board_mod_font to 80% @default_forum_text_font_family to be consistent
- Set @board_sub_font to 80% @default_forum_text_font_family to be consistent
- Set .boards .main width to auto
- Removed @board_align_posts
- Changed @board_align_threads to @board_align_count
- Made .boards .threads and .boards .posts same width
- Styled .boards .threads and .boards .posts with text-align: @board_align_count
- Moved "by $[board.last_thread.last_post.created_by]" next to recent post link rather than under it on Board List layout template
- Changed .description, .moderators, and .sub-boards on Board List layout from paragraph tags to div tags
- Removed legend and stats table
- Removed "Board, Threads, Posts, Last Post" row from Board List layout template
- Added "threads" and "posts" label under associated numbers to Board List layout template

post list ---
- Added script to remove default inline styles from thread description plugin because they were !important and could not be overwritten through the stylesheet
- Appended .thread_description_page to .messages .participants CSS rule to make them the same
- Fixed padding on control bar items
- Styled .posts span.labels with padding: 0 6px 4px 6px to adjust spacing between borders

messages list ---
- Styled .messages .item > td with border-width: 0 to remove extra inner 1px border on far right in Message List layout template
- Set .messages .participants to only have bottom border
- Added .last to <th class="latest"> to remove extra inner 1px border on far right in Conversations Page layout template
- Styled .conversations .main with text-align: @conversation_align_subject; to make it consistent with thread list
