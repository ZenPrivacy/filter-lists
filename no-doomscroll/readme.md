# no-doomscroll

![Human hours saved](https://img.shields.io/badge/human_hours_saved-%E2%88%9E-blue)
![Contributions are welcome](https://img.shields.io/badge/contributions-welcome-green)

`no-doomscroll` is an opinionated set of ad-block filter lists that hide algorithmic feeds, recommendations, and other UI elements designed to keep you scrolling.

Covers YouTube, TikTok, Instagram, X, Reddit, Bluesky, LinkedIn, and Twitch. Works with [Zen](https://github.com/ZenPrivacy/zen-desktop) and [uBlock Origin](https://github.com/gorhill/uBlock).


<p align="center">
  <picture>
    <img src="./showcase.gif?raw=true" width="800" alt="Animated demonstration showing no-doomscroll in action across multiple sites. YouTube, Reddit, X (Twitter), Twitch, and TikTok are displayed first in their default states, then with no-doomscroll enabled with hidden feeds and other distracting elements."  />
  </picture>
</p>

## How to add

The lists are compatible with [Zen](https://github.com/ZenPrivacy/zen-desktop) and [uBlock Origin](https://github.com/gorhill/uBlock).

| Ad-blocker | Instructions |
|---------|--------------|
| Zen | Available in Zen under **Filter lists → Digital wellbeing** |
| uBlock Origin | Open Dashboard → Filter lists → Import → Add the filter list URL |

Subscribe to **All sites** to cover everything, or pick individual sites if you only want to control specific platforms.

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
| Twitch | [Link](https://cdn.jsdelivr.net/gh/ZenPrivacy/filter-lists@master/no-doomscroll/twitch/main-zen.txt) | Home page, recommended channels, categories |

## Something broke?

Social media sites ship UI changes constantly, so the lists can break. If a feed reappears or a page looks wrong, [file an issue](https://github.com/ZenPrivacy/filter-lists/issues/new?labels=no-doomscroll) with:

- The site and page URL.
- What you're seeing that shouldn't be there (or what's missing that should still work).
- Screenshots (preferably).
- Your browser and ad-blocker.

Filter lists update every 12 hours, so please allow some time for fixes to propagate.

## Contributing

Contributions are welcome – whether it's fixing a broken filter, improving coverage on an existing site, or adding a new platform entirely.

- Each site has its own file under `no-doomscroll/<site>/main-zen.txt`. The combined list at [`no-doomscroll/main-zen.txt`](main-zen.txt) includes them all.
- The goal is to block feeds and recommendations, not content. If a user navigated there on purpose, it should still work.
- Test your filters in both Zen and uBlock Origin.

Open a [pull request](https://github.com/ZenPrivacy/filter-lists/pulls) with the label `no-doomscroll`.
