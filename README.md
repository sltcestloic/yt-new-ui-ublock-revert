# yt-new-ui-ublock-revert

Copy / paste into uBlock origin > dashboard > My filters

Most of those are from https://lifehacker.com/tech/how-to-undo-youtubes-terrible-new-layout, I added a few lines to remove the the comment teaser and the buttons I don't use

```
! Youtube New UI Fix

! Related videos
youtube.com###related #thumbnail.ytd-rich-grid-media:style(margin-right: 8px!important;height: 94px!important;width: 168px!important;min-width: 168px!important;)
youtube.com###related #avatar-link.ytd-rich-grid-media, #related #attached-survey.ytd-rich-grid-media, #related .ytd-rich-shelf-renderer .button-container.ytd-rich-shelf-renderer:style(display:none!important;)
youtube.com###related #dismissible.ytd-rich-grid-media:style(display:flex;flex-direction:row!important;)
youtube.com###related #details.ytd-rich-grid-media:style(width: 100%!important;min-width: 0!important;)
youtube.com###related #contents ytd-rich-item-renderer:style(margin:0!important;margin-top:8px!important;)
youtube.com###related ytd-rich-grid-row #contents.ytd-rich-grid-row,#related h3.ytd-rich-grid-media,#related ytd-rich-section-renderer #content,#related #rich-shelf-header.ytd-rich-shelf-renderer:style(margin:0!important;)
youtube.com###related ytd-rich-item-renderer.ytd-rich-grid-row,#content.ytd-rich-item-renderer:style(width:100%!important;)
youtube.com###related #video-title.ytd-rich-grid-media:style(font-size:1.4rem!important;)
youtube.com###related .ytd-channel-name a,#related #metadata-line.ytd-video-meta-block span:style(font-size:12px!important;)
youtube.com###related ytd-rich-grid-renderer #contents:style(padding-top:0px!important;)
youtube.com###related .ytd-rich-shelf-renderer ytd-rich-item-renderer.ytd-rich-shelf-renderer:style(width:130px!important;min-width: 130px!important;)
youtube.com###related #contents.ytd-rich-shelf-renderer:style(display: flex !important;flex-direction: row !important;gap: 8px !important;flex-wrap: nowrap!important;max-width: 400px!important;overflow-x: scroll!important;overflow-y: hidden!important)
youtube.com###related .ytd-rich-shelf-renderer .yt-core-image:style(object-fit: cover!important;)
youtube.com###related ytd-rich-section-renderer #contents:style(margin-left:0!important)
youtube.com###related #contents ytd-rich-section-renderer ytd-rich-item-renderer:style(margin-top:0px!important;)
youtube.com###related .ytd-rich-shelf-renderer ytd-rich-item-renderer.ytd-rich-shelf-renderer[hidden=""]:style(display:block!important;)
youtube.com###related #dismissible.ytd-rich-shelf-renderer:style(margin:0!important; border-color: transparent!important)

! Title
youtube.com###title yt-formatted-string.ytd-watch-metadata:style(font-size:20px!important; font-weight: 700!important; line-height:28px!important)

! Comment teaser
youtube.com###comment-teaser:style(display: none)

! Download / thanks / clip buttons
youtube.com###flexible-item-buttons:style(display: none)

! New UI js flags
youtube.com##+js(set, yt.config_.EXPERIMENT_FLAGS.kevlar_watch_grid, false)
youtube.com##+js(set, yt.config_.EXPERIMENT_FLAGS.small_avatars_for_comments, false)
youtube.com##+js(set, yt.config_.EXPERIMENT_FLAGS.kevlar_watch_comments_panel_button, false)
youtube.com##+js(set, yt.config_.EXPERIMENT_FLAGS.web_rounded_thumbnails, false)
youtube.com##+js(set, yt.config_.EXPERIMENT_FLAGS.web_watch_rounded_player_large, false)
youtube.com##+js(set, yt.config_.EXPERIMENT_FLAGS.kevlar_watch_max_player_width, 1280)
```
