# no-doomscroll

![Human hours saved](https://img.shields.io/badge/human_hours_saved-%E2%88%9E-blue)
![Contributions are welcome](https://img.shields.io/badge/contributions-welcome-green)

RESIST. Reclaim your attention. Reclaim your life.

Every major social platform employs an algorithmic feed tuned to maximize the time you spend on it – not the value you get from it. The "For You" page, the infinite home feed, the autoplay queue, the "you might also like" sidebar – none of these exist for your benefit. They exist because your attention is the product.

`no-doomscroll` is an opinionated set of filter lists that remove these feeds, recommendations, and other bits of UI whose only job is to keep you scrolling. You can still open a profile, read a post, message a friend, or look something up – the only thing that disappears is the endless stream you never asked for.

## How to add

The filter lists are compatible with [Zen](https://github.com/ZenPrivacy/zen-desktop) and [uBlock Origin](https://github.com/gorhill/uBlock).

| Ad-blocker | Instructions |
|---------|--------------|
| Zen | Open Filter lists → Custom → Add the filter list URL |
| uBlock Origin | Open Dashboard → Filter lists → Import → Add the filter list URL |

You can subscribe to the **All sites** list to cover everything, or pick individual sites if you only want to control specific platforms.

## Filter lists

| List | Link | What's blocked |
|------|------|----------------|
| __All sites (combined)__ | [Link](https://cdn.jsdelivr.net/gh/ZenPrivacy/filter-lists@master/no-doomscroll/main-zen.txt) | Everything below, combined |
| YouTube | [Link](https://cdn.jsdelivr.net/gh/ZenPrivacy/filter-lists@master/no-doomscroll/youtube/main-zen.txt) | Home feed, Shorts, sidebar recommendations, end-screen suggestions, Explore section, notification bell |
| TikTok | [Link](https://cdn.jsdelivr.net/gh/ZenPrivacy/filter-lists@master/no-doomscroll/tiktok/main-zen.txt) | For You, Explore, and Following feeds and sidebar links |
| Instagram | [Link](https://cdn.jsdelivr.net/gh/ZenPrivacy/filter-lists@master/no-doomscroll/instagram/main-zen.txt) | Home, Explore, Suggested People, Reels |
| X | [Link](https://cdn.jsdelivr.net/gh/ZenPrivacy/filter-lists@master/no-doomscroll/x/main-zen.txt) | Home and Explore feeds; sidebar Today's News, What's happening, Who to follow |
| Reddit | [Link](https://cdn.jsdelivr.net/gh/ZenPrivacy/filter-lists@master/no-doomscroll/reddit/main-zen.txt) | Home, r/popular, r/all, and r/explore feeds; recent posts |
| Bluesky | [Link](https://cdn.jsdelivr.net/gh/ZenPrivacy/filter-lists@master/no-doomscroll/bluesky/main-zen.txt) | Custom and Following feeds on index page |
| LinkedIn | [Link](https://cdn.jsdelivr.net/gh/ZenPrivacy/filter-lists@master/no-doomscroll/linkedin/main-zen.txt) | Feed posts, news module, follows suggestions, right sidebar, games |
| Twitch | [Link](https://cdn.jsdelivr.net/gh/ZenPrivacy/filter-lists@master/no-doomscroll/twitch/main-zen.txt) | Recommended channels, categories |

## Something broke?

Social media sites ship UI changes constantly, and when they do, selectors can go stale. If a feed reappears or a page looks wrong, [file an issue](https://github.com/ZenPrivacy/filter-lists/issues/new?labels=no-doomscroll) with:

- The site and page URL.
- What you're seeing that shouldn't be there (or what's missing that should still work).
- Screenshots (preferably).
- Your browser and ad-blocker.

Filter lists update every 12 hours, so please allow some time for fixes to propagate.

## Contributing

Contributions are welcome – whether it's fixing a broken filter, improving coverage on an existing site, or adding a new platform entirely.

- Each site has its own file under `no-doomscroll/<site>/main-zen.txt`. The combined list in `no-doomscroll/main-zen.txt` just includes them all.
- The goal is to block feeds and recommendation feeds, not content. If a user navigated there on purpose, it should still work.
- Test your filters in both Zen and uBlock Origin.

Open a [pull request](https://github.com/ZenPrivacy/filter-lists/pulls) with the label `no-doomscroll`.
