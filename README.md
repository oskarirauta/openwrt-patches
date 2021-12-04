## openwrt-patches

### Patch repository for OpenWRT

This repository contains mostly patches to OpenWRT which are not included in mainstream. They are not supposed to be used, unless they provide a fix to issue; if there is no issue, skip patch. Or they add some functionality which is slimmed down for downsizing to allow usage on embedded platforms - but sometimes, you need more.

All patches here should be optional, used when needed, instead of _collect 'em all.._

### Patching

Patches are supposed to be used in root of each tree. When patches are created, they are for current master branch of each category, or atleast for reasonably recent snapshot..

Patches are ordered by category, under packages.git, you find patches agains Openwrt's packages feed.

Readme of available category lists patches, and what they do. If patch's name contains _PR#####_ - it means there was a PR done against repository, but patch is now here because it was rejected and _PR#####_ in name is a reference to that PR, which might contain extended explanation of issue or feature. I also try add some details to patches comment section at top of patch file, but I cannot fully focus on just maintaining this repository, so I might forget to do that sometimes, sorry in advance.

If there is multiple patches with same name, ending with -001, -002, -003 it means that patch is splitted to multiple files (I try to avoid this, but if patch is huge, it's easier to follow it when it's splitted), and numbers are correct order to use when patching.

### Maintenance

Patches might not be tested that they work on recent branches, so they might get _old_. If I notice that something has been fixed in mainstream, I will remove that patch as unnecessary. Even though patch might be old, it maybe isn't useless, as even though it would fail, it might be just enough to ease your pain when you do not need to re-invent the wheel; just need to patch manually ackordingly to old patch..

### Contribution

I add patches when I find something to patch and it won't be accepted to mainstream for purposes such as _rare issue_ or _not easy to replicate_. I also accept pull requests- for completely new patches, and for renewals of old patches. Guidelines for acceptance of PR's is that common sense must be used, patch should serve the crowd, not invidual person, so don't hardcode it to suite just you; and when patching- add your contact info to patches comment section and when committing, sign off it also for same contact info. And ofcourse, in the pr.. Let me know what it is for.. But keep in mind, that this is not a package repository; so avoid new software packages, these patches are used against existing contents of category, whether is was to fix issues, or add improvement or features- also if you want to update some software, PR should atleast first go to mainstream, not here...
