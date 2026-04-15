# pmm-ci-hackathon
PMM competitive intelligence hackathon

## 4 Modes & data points

### 🏗️ Product Mode
Source: product pages, docs, changelog, feature listings, integrations page
- Product and feature names + descriptions
- Feature categories (e.g. data extraction, proxy, scheduling, AI agents)
- Integrations listed (Zapier, Make, REST API, SDKs, etc.)
- SDK / language support (Python, JS, etc.)
- Changelog entries — date + what changed
- Documentation structure (topics covered = what they think matters)
- Free tier / trial availability (yes/no + limits if stated)
- Tech stack signals visible from docs or job listings

### 📣 Marketing Mode
Source: homepage, blog, YouTube, Facebook Ad Library, X/Twitter, Instagram, Facebook, LinkedIn (to be added later)

**Website & Positioning** — https://apify.com/apify/website-content-crawler:
- Hero headline + subheadline (exact copy)
- Primary value proposition / positioning statement
- Target personas mentioned or implied
- Use cases promoted (e.g. price monitoring, lead generation, AI training data)
- Industries / verticals highlighted

**Content** — https://apify.com/apify/website-content-crawler:
- Blog post titles + publish dates + categories
- Blog posting frequency (posts per month)
- YouTube video titles + publish dates + view counts

**Ads** — https://apify.com/apify/facebook-ads-scraper:
- Active ad creatives from Facebook Ad Library — headline, CTA, visual format, copy

**Social Media:**
- X/Twitter: recent posts, posting frequency, engagement signals
- Instagram: content themes, posting frequency
- Facebook: page activity signals
- LinkedIn: (to be connected later — scraper `kfiWbq3boy3dWKbiL` identified, requires LinkedIn cookies setup)

### 🤑 Sales Mode
Source: Job boards, Glassdoor, BuiltWith, Crunchbase, LinkedIn

**Job Boards (Google Jobs, Indeed, Lever):**
- Hiring velocity (ratio of sales roles vs. engineering roles)
- Target personas and territories (e.g., Enterprise focus in EMEA)
- Sales methodology (MEDDIC, Challenger, or other frameworks mentioned)
- Sales team composition (headcount distribution across SDR, AE, and CS)

**Glassdoor:**
- Internal red flags (product-sales gap, implementation delays)
- Sales culture and turnover signals
- Negotiation behavior (mentions of discounting or contract flexibility)
- Talent positioning (how they pitch the company vision to hires)

**Technographic Tools (BuiltWith, Wappalyzer):**
- Tech stack alignment (tools they commonly replace or integrate with)
- Customer sophistication signals (complexity of the tech stack they sell into)
- Premium integration hooks (identifying enterprise-only connectors)

**Corporate & Business (Crunchbase, LinkedIn):**
- Growth signals (funding rounds, acquisitions, strategic shifts)
- Leadership turnover (tracking VP/C-level changes in sales/marketing)
- Geographic expansion (headcount shifts in new regions)

### 💰 Pricing Mode
Source: pricing page (public); product-specific pricing page if product name is specified
- Plan names
- Plan prices (monthly + annual where available)
- Key limits per plan (API calls, seats, requests, GB, etc.)
- Overage / pay-as-you-go rates
- Free tier details (what's included, limits)
- Trial availability + duration
- Enterprise tier (exists yes/no, contact-sales gating)
- API pricing (separate page or bundled into plans)
- Billing model (seat-based, usage-based, flat, hybrid)
- If `product_name` is provided → scrapes that product's specific pricing page instead of company-wide

### 👥 Customer Mode
Source: G2, Capterra, Product Hunt, GitHub, Reddit, website testimonials

**Review Platforms (G2, Capterra):**
- Overall rating + review count
- Rating breakdown by category (ease of use, support, value, features)
- Common pros mentioned (extracted themes)
- Common cons / complaints (extracted themes)
- Use cases reviewers describe
- Reviewer personas — job title, company size, industry (where available)

**Product Hunt:**
- Upvote count
- Top comments sentiment
- What people highlight as love/hate

**GitHub:**
- Star count
- Open issues count
- Recent issue themes / sentiment
- Contributor activity signals

**Website Testimonials:**
- Company name
- Quote snippet
- Use case described

**Reddit:**
- Mention frequency
- Sentiment signal

## Actor mapping by user need

| User Need | Actor ID | Best For |
|---|---|---|
| Competitor business data | `compass/crawler-google-places` | Location analysis |
| Competitor contact discovery | `poidata/google-maps-email-extractor` | Email extraction |
| Feature benchmarking | `compass/google-maps-extractor` | Detailed business data |
| Competitor review analysis | `compass/Google-Maps-Reviews-Scraper` | Review comparison |
| Hotel competitor data | `voyager/booking-scraper` | Hotel benchmarking |
| Hotel review comparison | `voyager/booking-reviews-scraper` | Review analysis |
| Competitor ad strategies | `apify/facebook-ads-scraper` | Ad creative analysis |
| Competitor page metrics | `apify/facebook-pages-scraper` | Page performance |
| Competitor content analysis | `apify/facebook-posts-scraper` | Post strategies |
| Competitor reels performance | `apify/facebook-reels-scraper` | Reels analysis |
| Competitor audience analysis | `apify/facebook-comments-scraper` | Comment sentiment |
| Competitor event monitoring | `apify/facebook-events-scraper` | Event tracking |
| Competitor audience overlap | `apify/facebook-followers-following-scraper` | Follower analysis |
| Competitor review benchmarking | `apify/facebook-reviews-scraper` | Review comparison |
| Competitor ad monitoring | `apify/facebook-search-scraper` | Ad discovery |
| Competitor profile metrics | `apify/instagram-profile-scraper` | Profile analysis |
| Competitor content monitoring | `apify/instagram-post-scraper` | Post tracking |
| Competitor engagement analysis | `apify/instagram-comment-scraper` | Comment analysis |
| Competitor reel performance | `apify/instagram-reel-scraper` | Reel metrics |
| Competitor growth tracking | `apify/instagram-followers-count-scraper` | Follower tracking |
| Comprehensive competitor data | `apify/instagram-scraper` | Full analysis |
| API-based competitor analysis | `apify/instagram-api-scraper` | API access |
| Competitor video analysis | `streamers/youtube-scraper` | Video metrics |
| Competitor sentiment analysis | `streamers/youtube-comments-scraper` | Comment sentiment |
| Competitor channel metrics | `streamers/youtube-channel-scraper` | Channel analysis |
| TikTok competitor analysis | `clockworks/tiktok-scraper` | TikTok data |
| Competitor video strategies | `clockworks/tiktok-video-scraper` | Video analysis |
| Competitor TikTok profiles | `clockworks/tiktok-profile-scraper` | Profile data |

