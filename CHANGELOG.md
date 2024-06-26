## Changelog
 - Version 2.12.2 [2024-04-20]
   - New Feature #11: Support for Movies & TV Shows is finally here.
   - AnimePahe: Reload saved cookies for faster loading.
   - Several optimizations under the hood.

 - Version 2.11.6 [2024-03-24]
   - Fix update issue - unable to retrieve info from Git
   - Dynamically fetch the cdn url for GogoAnime Client instead of config file.
   - Updated GogoAnime Link in Config.
   - Corrected few typos.

 - Version 2.11.3 [2024-02-11]
   - Feature: Display download size of stream video files. The accuracy of size estimation can be tuned by setting -hsa [percent]. Disabled by default.
   - Feature: Select specific episodes in addition to a range of episodes. Examples of valid inputs: 1,3,5 | 1-4,6 | 5 | 1-5 | 1- | -3
   - Added License & Updated Readme (with UDB demo)
   - Fix minor bug in DramaClient

 - Version 2.11.2 [2024-01-28]
   - Implemented Feature #8: Support for GogoAnime.
   - The UDB interface is now vibrant with colors. Explore the enhanced cli visual experience!
   - Introduced an option to update UDB directly within the application.
   - Added a new feature to display video duration information.
   - Included performance enhancements and addressed minor bugs for a smoother user experience.

 - Version 2.10.6 [2024-01-18]
   - Fix #9: import error for Crypto.Cipher with pycryptodome. Replaced pycryptodome with pycryptodomex.

 - Version 2.10.5 [2024-01-17]
   - Fix #7: Bypass DDoS check in AnimePahe (requires undetected chromedriver)
   - Show total episodes count for a drama in search results
   - Minor bug fixes

 - Version 2.10.3 [2023-11-06]
   - Updated Anime Client as per new APIs
   - Updated Drama Client to fetch single m3u8 links
   - Optimized HLS Downloader to fetch segment links

 - Version 2.10.0 [2023-10-07]
   - Added new Downloader for non-m3u8 links 🎉
   - Fixed #5
   - Optimized Downloader under the hood

 - Version 2.9.0 [2023-10-06]
   - Changed to Semantic versioning
   - Implemented version check
   - Bug fixes #4 #5
   - Show skipped episodes in download summary

 - Version 2.8 [2023-10-04]
   - Added detailed loggers to make it developer friendly :)
   - Updated drama links
   - Get stream links dynamically
   - Updated _fetch_episodes_list_ in Drama to load episodes > 50
   - Added option to auto select from available resolutions
   - Performance optimizations under the hood

 - Version 2.7 [2023-06-05]
   - Added CLI support for automation. Run this command for details: `python udb.py -h`
   - Added dynamic output declaration
   - Fixed downloading of floating episodes (ex: 6.5, 10.5)

 - Version 2.6 [2023-05-20]
   - Added Linux OS compatibility
   - Fixed unable to load X.5 episodes

 - Version 2.5 [2023-04-12]
   - Modified anime client as per updated animepahe site
   - Added support for backup url in Dramas
   - Added support for non-ts m3u8 urls
   - Add preferred & blacklist of m3u8 links
   - Removed dependency on openssl. Uses pycryptodome instead

 - Version 2.0 [2023-02-11]
   - Rewritten code completely
   - Added support to download drama. Finally.. ^_^
   - Added support to retrieve paginated episodes from AnimePahe
   - Added headers & custom retry decorator while downloading segments to avoid Connection Reset Error
   - Generalized parallel downloader
   - Added Progress bar for downloads using tqdm

 - Version 1.5 [2023-02-02]
   - All new downloader. Custom implementation of m3u8 downloader and reliable m3u8 parser

 - Version 1.2 [2023-01-29]
   - Fix m3u8 link parser. Bug fixes

 - Version 1.1 [2023-01-28]
   - First version
   - Download multiple anime episodes in parallel from animepahe
