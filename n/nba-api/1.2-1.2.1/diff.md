# Comparing `tmp/nba_api-1.2.tar.gz` & `tmp/nba_api-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nba_api-1.2.tar", max compression
+gzip compressed data, was "nba_api-1.2.1.tar", max compression
```

## Comparing `nba_api-1.2.tar` & `nba_api-1.2.1.tar`

### file list

```diff
@@ -1,166 +1,166 @@
--rw-r--r--   0        0        0     1088 2022-09-09 10:27:55.158978 nba_api-1.2/LICENSE
--rw-r--r--   0        0        0     1159 2023-03-23 21:23:27.977159 nba_api-1.2/pyproject.toml
--rw-r--r--   0        0        0     4420 2022-11-16 12:11:59.294578 nba_api-1.2/README.md
--rw-r--r--   0        0        0       18 2022-10-09 01:59:25.616191 nba_api-1.2/src/nba_api/__init__.py
--rw-r--r--   0        0        0        0 2022-10-09 01:59:25.617190 nba_api-1.2/src/nba_api/library/__init__.py
--rw-r--r--   0        0        0        0 2022-10-09 01:59:25.617190 nba_api-1.2/src/nba_api/library/debug/__init__.py
--rw-r--r--   0        0        0      192 2022-10-09 01:59:25.617190 nba_api-1.2/src/nba_api/library/debug/debug.py
--rw-r--r--   0        0        0     4288 2023-02-10 02:29:33.203040 nba_api-1.2/src/nba_api/library/http.py
--rw-r--r--   0        0        0        2 2022-10-09 01:59:25.618187 nba_api-1.2/src/nba_api/live/__init__.py
--rw-r--r--   0        0        0        0 2022-10-09 01:59:25.618187 nba_api-1.2/src/nba_api/live/nba/__init__.py
--rw-r--r--   0        0        0      178 2022-10-09 01:59:25.618187 nba_api-1.2/src/nba_api/live/nba/endpoints/__init__.py
--rw-r--r--   0        0        0      601 2022-10-09 01:59:25.619186 nba_api-1.2/src/nba_api/live/nba/endpoints/_base.py
--rw-r--r--   0        0        0     9894 2022-10-09 01:59:25.619186 nba_api-1.2/src/nba_api/live/nba/endpoints/boxscore.py
--rw-r--r--   0        0        0     2534 2022-10-09 01:59:25.619186 nba_api-1.2/src/nba_api/live/nba/endpoints/playbyplay.py
--rw-r--r--   0        0        0     2484 2022-10-09 01:59:25.619186 nba_api-1.2/src/nba_api/live/nba/endpoints/scoreboard.py
--rw-r--r--   0        0        0        0 2022-10-09 01:59:25.620186 nba_api-1.2/src/nba_api/live/nba/library/__init__.py
--rw-r--r--   0        0        0     1043 2022-10-09 01:59:25.620186 nba_api-1.2/src/nba_api/live/nba/library/http.py
--rw-r--r--   0        0        0        0 2022-10-09 01:59:25.620186 nba_api-1.2/src/nba_api/stats/__init__.py
--rw-r--r--   0        0        0    10950 2023-03-23 21:24:17.858394 nba_api-1.2/src/nba_api/stats/endpoints/__init__.py
--rw-r--r--   0        0        0     2275 2022-10-09 01:59:25.621191 nba_api-1.2/src/nba_api/stats/endpoints/_base.py
--rw-r--r--   0        0        0     4331 2022-10-09 01:59:25.621191 nba_api-1.2/src/nba_api/stats/endpoints/alltimeleadersgrids.py
--rw-r--r--   0        0        0     1956 2022-10-09 01:59:25.621191 nba_api-1.2/src/nba_api/stats/endpoints/assistleaders.py
--rw-r--r--   0        0        0     4820 2022-10-09 01:59:25.621191 nba_api-1.2/src/nba_api/stats/endpoints/assisttracker.py
--rw-r--r--   0        0        0     2771 2022-10-09 01:59:25.622186 nba_api-1.2/src/nba_api/stats/endpoints/boxscoreadvancedv2.py
--rw-r--r--   0        0        0     1830 2022-10-09 01:59:25.622186 nba_api-1.2/src/nba_api/stats/endpoints/boxscoredefensive.py
--rw-r--r--   0        0        0     2515 2022-10-09 01:59:25.622186 nba_api-1.2/src/nba_api/stats/endpoints/boxscorefourfactorsv2.py
--rw-r--r--   0        0        0     2044 2022-10-09 01:59:25.623187 nba_api-1.2/src/nba_api/stats/endpoints/boxscorematchups.py
--rw-r--r--   0        0        0     2547 2022-10-09 01:59:25.623187 nba_api-1.2/src/nba_api/stats/endpoints/boxscoremiscv2.py
--rw-r--r--   0        0        0     2000 2022-10-09 01:59:25.623187 nba_api-1.2/src/nba_api/stats/endpoints/boxscoreplayertrackv2.py
--rw-r--r--   0        0        0     2729 2022-10-09 01:59:25.623187 nba_api-1.2/src/nba_api/stats/endpoints/boxscorescoringv2.py
--rw-r--r--   0        0        0     2335 2022-10-09 01:59:25.624186 nba_api-1.2/src/nba_api/stats/endpoints/boxscoresimilarityscore.py
--rw-r--r--   0        0        0     3686 2022-10-09 01:59:25.624186 nba_api-1.2/src/nba_api/stats/endpoints/boxscoresummaryv2.py
--rw-r--r--   0        0        0     2891 2022-10-09 01:59:25.624186 nba_api-1.2/src/nba_api/stats/endpoints/boxscoretraditionalv2.py
--rw-r--r--   0        0        0     2647 2022-10-09 01:59:25.624186 nba_api-1.2/src/nba_api/stats/endpoints/boxscoreusagev2.py
--rw-r--r--   0        0        0     1899 2022-10-09 01:59:25.625186 nba_api-1.2/src/nba_api/stats/endpoints/commonallplayers.py
--rw-r--r--   0        0        0     2335 2022-10-09 01:59:25.625186 nba_api-1.2/src/nba_api/stats/endpoints/commonplayerinfo.py
--rw-r--r--   0        0        0     1710 2022-10-09 01:59:25.625186 nba_api-1.2/src/nba_api/stats/endpoints/commonplayoffseries.py
--rw-r--r--   0        0        0     1999 2022-10-09 01:59:25.626188 nba_api-1.2/src/nba_api/stats/endpoints/commonteamroster.py
--rw-r--r--   0        0        0     1509 2022-10-09 01:59:25.626188 nba_api-1.2/src/nba_api/stats/endpoints/commonteamyears.py
--rw-r--r--   0        0        0     2793 2022-10-09 01:59:25.626188 nba_api-1.2/src/nba_api/stats/endpoints/cumestatsplayer.py
--rw-r--r--   0        0        0     2428 2022-10-09 01:59:25.627187 nba_api-1.2/src/nba_api/stats/endpoints/cumestatsplayergames.py
--rw-r--r--   0        0        0     2850 2022-10-09 01:59:25.627187 nba_api-1.2/src/nba_api/stats/endpoints/cumestatsteam.py
--rw-r--r--   0        0        0     2502 2022-10-09 01:59:25.627187 nba_api-1.2/src/nba_api/stats/endpoints/cumestatsteamgames.py
--rw-r--r--   0        0        0     3591 2022-10-09 01:59:25.628188 nba_api-1.2/src/nba_api/stats/endpoints/defensehub.py
--rw-r--r--   0        0        0     2315 2022-10-09 01:59:25.628188 nba_api-1.2/src/nba_api/stats/endpoints/draftboard.py
--rw-r--r--   0        0        0     1784 2022-10-09 01:59:25.629188 nba_api-1.2/src/nba_api/stats/endpoints/draftcombinedrillresults.py
--rw-r--r--   0        0        0     2461 2022-10-09 01:59:25.629188 nba_api-1.2/src/nba_api/stats/endpoints/draftcombinenonstationaryshooting.py
--rw-r--r--   0        0        0     1860 2022-10-09 01:59:25.629188 nba_api-1.2/src/nba_api/stats/endpoints/draftcombineplayeranthro.py
--rw-r--r--   0        0        0     2841 2022-10-09 01:59:25.630187 nba_api-1.2/src/nba_api/stats/endpoints/draftcombinespotshooting.py
--rw-r--r--   0        0        0     2631 2022-10-09 01:59:25.630187 nba_api-1.2/src/nba_api/stats/endpoints/draftcombinestats.py
--rw-r--r--   0        0        0     2304 2022-10-09 01:59:25.631189 nba_api-1.2/src/nba_api/stats/endpoints/drafthistory.py
--rw-r--r--   0        0        0     3695 2022-10-09 01:59:25.631189 nba_api-1.2/src/nba_api/stats/endpoints/fantasywidget.py
--rw-r--r--   0        0        0     1939 2022-10-09 01:59:25.631189 nba_api-1.2/src/nba_api/stats/endpoints/franchisehistory.py
--rw-r--r--   0        0        0     1766 2022-10-09 01:59:25.632187 nba_api-1.2/src/nba_api/stats/endpoints/franchiseleaders.py
--rw-r--r--   0        0        0     2029 2022-10-09 01:59:25.632187 nba_api-1.2/src/nba_api/stats/endpoints/franchiseplayers.py
--rw-r--r--   0        0        0     1906 2022-10-09 01:59:25.632187 nba_api-1.2/src/nba_api/stats/endpoints/gamerotation.py
--rw-r--r--   0        0        0     2374 2022-10-09 01:59:25.633189 nba_api-1.2/src/nba_api/stats/endpoints/glalumboxscoresimilarityscore.py
--rw-r--r--   0        0        0     2609 2022-10-09 01:59:25.633189 nba_api-1.2/src/nba_api/stats/endpoints/homepageleaders.py
--rw-r--r--   0        0        0     3313 2022-10-09 01:59:25.633189 nba_api-1.2/src/nba_api/stats/endpoints/homepagev2.py
--rw-r--r--   0        0        0     2455 2022-10-09 01:59:25.634191 nba_api-1.2/src/nba_api/stats/endpoints/hustlestatsboxscore.py
--rw-r--r--   0        0        0     1737 2022-10-09 01:59:25.634191 nba_api-1.2/src/nba_api/stats/endpoints/infographicfanduelplayer.py
--rw-r--r--   0        0        0     2667 2022-10-09 01:59:25.634191 nba_api-1.2/src/nba_api/stats/endpoints/leaderstiles.py
--rw-r--r--   0        0        0     4975 2022-10-09 01:59:25.635188 nba_api-1.2/src/nba_api/stats/endpoints/leaguedashlineups.py
--rw-r--r--   0        0        0     4608 2022-10-09 01:59:25.635188 nba_api-1.2/src/nba_api/stats/endpoints/leaguedashoppptshot.py
--rw-r--r--   0        0        0     5445 2022-10-09 01:59:25.635188 nba_api-1.2/src/nba_api/stats/endpoints/leaguedashplayerbiostats.py
--rw-r--r--   0        0        0     6551 2022-10-09 01:59:25.636187 nba_api-1.2/src/nba_api/stats/endpoints/leaguedashplayerclutch.py
--rw-r--r--   0        0        0     5660 2022-10-09 01:59:25.636187 nba_api-1.2/src/nba_api/stats/endpoints/leaguedashplayerptshot.py
--rw-r--r--   0        0        0     6087 2022-10-09 01:59:25.636187 nba_api-1.2/src/nba_api/stats/endpoints/leaguedashplayershotlocations.py
--rw-r--r--   0        0        0     6299 2022-10-09 01:59:25.637186 nba_api-1.2/src/nba_api/stats/endpoints/leaguedashplayerstats.py
--rw-r--r--   0        0        0     5132 2022-10-09 01:59:25.637186 nba_api-1.2/src/nba_api/stats/endpoints/leaguedashptdefend.py
--rw-r--r--   0        0        0     5061 2022-10-09 01:59:25.637186 nba_api-1.2/src/nba_api/stats/endpoints/leaguedashptstats.py
--rw-r--r--   0        0        0     3988 2022-10-09 01:59:25.638185 nba_api-1.2/src/nba_api/stats/endpoints/leaguedashptteamdefend.py
--rw-r--r--   0        0        0     5884 2022-10-09 01:59:25.638185 nba_api-1.2/src/nba_api/stats/endpoints/leaguedashteamclutch.py
--rw-r--r--   0        0        0     4610 2022-10-09 01:59:25.638185 nba_api-1.2/src/nba_api/stats/endpoints/leaguedashteamptshot.py
--rw-r--r--   0        0        0     5520 2022-10-09 01:59:25.638185 nba_api-1.2/src/nba_api/stats/endpoints/leaguedashteamshotlocations.py
--rw-r--r--   0        0        0     5645 2022-10-09 01:59:25.639185 nba_api-1.2/src/nba_api/stats/endpoints/leaguedashteamstats.py
--rw-r--r--   0        0        0     9785 2022-10-09 01:59:25.639185 nba_api-1.2/src/nba_api/stats/endpoints/leaguegamefinder.py
--rw-r--r--   0        0        0     2545 2022-10-09 01:59:25.639185 nba_api-1.2/src/nba_api/stats/endpoints/leaguegamelog.py
--rw-r--r--   0        0        0     4768 2022-10-09 01:59:25.640186 nba_api-1.2/src/nba_api/stats/endpoints/leaguehustlestatsplayer.py
--rw-r--r--   0        0        0     5447 2022-10-09 01:59:25.640186 nba_api-1.2/src/nba_api/stats/endpoints/leaguehustlestatsplayerleaders.py
--rw-r--r--   0        0        0     4614 2022-10-09 01:59:25.640186 nba_api-1.2/src/nba_api/stats/endpoints/leaguehustlestatsteam.py
--rw-r--r--   0        0        0     5424 2022-10-09 01:59:25.641187 nba_api-1.2/src/nba_api/stats/endpoints/leaguehustlestatsteamleaders.py
--rw-r--r--   0        0        0     2335 2022-10-09 01:59:25.641187 nba_api-1.2/src/nba_api/stats/endpoints/leagueleaders.py
--rw-r--r--   0        0        0     4807 2022-10-09 01:59:25.641187 nba_api-1.2/src/nba_api/stats/endpoints/leaguelineupviz.py
--rw-r--r--   0        0        0     4440 2022-10-09 01:59:25.641187 nba_api-1.2/src/nba_api/stats/endpoints/leagueplayerondetails.py
--rw-r--r--   0        0        0     2572 2022-10-09 01:59:25.642186 nba_api-1.2/src/nba_api/stats/endpoints/leagueseasonmatchups.py
--rw-r--r--   0        0        0     2914 2022-10-09 01:59:25.642186 nba_api-1.2/src/nba_api/stats/endpoints/leaguestandings.py
--rw-r--r--   0        0        0     3788 2022-10-09 01:59:25.642186 nba_api-1.2/src/nba_api/stats/endpoints/leaguestandingsv3.py
--rw-r--r--   0        0        0     2503 2022-10-09 01:59:25.643190 nba_api-1.2/src/nba_api/stats/endpoints/matchupsrollup.py
--rw-r--r--   0        0        0     1935 2022-10-09 01:59:25.643190 nba_api-1.2/src/nba_api/stats/endpoints/playbyplay.py
--rw-r--r--   0        0        0     2380 2022-10-09 01:59:25.643190 nba_api-1.2/src/nba_api/stats/endpoints/playbyplayv2.py
--rw-r--r--   0        0        0     1547 2022-10-09 01:59:25.643190 nba_api-1.2/src/nba_api/stats/endpoints/playerawards.py
--rw-r--r--   0        0        0     2123 2022-10-09 01:59:25.644189 nba_api-1.2/src/nba_api/stats/endpoints/playercareerbycollege.py
--rw-r--r--   0        0        0     2822 2022-10-09 01:59:25.644189 nba_api-1.2/src/nba_api/stats/endpoints/playercareerbycollegerollup.py
--rw-r--r--   0        0        0     5370 2022-10-09 01:59:25.644189 nba_api-1.2/src/nba_api/stats/endpoints/playercareerstats.py
--rw-r--r--   0        0        0     4752 2022-10-09 01:59:25.645189 nba_api-1.2/src/nba_api/stats/endpoints/playercompare.py
--rw-r--r--   0        0        0    12845 2022-10-09 01:59:25.645189 nba_api-1.2/src/nba_api/stats/endpoints/playerdashboardbyclutch.py
--rw-r--r--   0        0        0     7841 2022-10-09 01:59:25.645189 nba_api-1.2/src/nba_api/stats/endpoints/playerdashboardbygamesplits.py
--rw-r--r--   0        0        0     9392 2022-10-09 01:59:25.646186 nba_api-1.2/src/nba_api/stats/endpoints/playerdashboardbygeneralsplits.py
--rw-r--r--   0        0        0     8578 2022-10-09 01:59:25.646186 nba_api-1.2/src/nba_api/stats/endpoints/playerdashboardbylastngames.py
--rw-r--r--   0        0        0     7020 2022-10-09 01:59:25.646186 nba_api-1.2/src/nba_api/stats/endpoints/playerdashboardbyopponent.py
--rw-r--r--   0        0        0     8237 2022-10-09 01:59:25.646186 nba_api-1.2/src/nba_api/stats/endpoints/playerdashboardbyshootingsplits.py
--rw-r--r--   0        0        0     7196 2022-10-09 01:59:25.647189 nba_api-1.2/src/nba_api/stats/endpoints/playerdashboardbyteamperformance.py
--rw-r--r--   0        0        0     5535 2022-10-09 01:59:25.647189 nba_api-1.2/src/nba_api/stats/endpoints/playerdashboardbyyearoveryear.py
--rw-r--r--   0        0        0     3658 2022-10-09 01:59:25.647189 nba_api-1.2/src/nba_api/stats/endpoints/playerdashptpass.py
--rw-r--r--   0        0        0     4817 2022-10-09 01:59:25.648186 nba_api-1.2/src/nba_api/stats/endpoints/playerdashptreb.py
--rw-r--r--   0        0        0     3440 2022-10-09 01:59:25.648186 nba_api-1.2/src/nba_api/stats/endpoints/playerdashptshotdefend.py
--rw-r--r--   0        0        0     5580 2022-10-09 01:59:25.648186 nba_api-1.2/src/nba_api/stats/endpoints/playerdashptshots.py
--rw-r--r--   0        0        0     2136 2022-10-09 01:59:25.648186 nba_api-1.2/src/nba_api/stats/endpoints/playerestimatedmetrics.py
--rw-r--r--   0        0        0     4068 2022-10-09 01:59:25.649190 nba_api-1.2/src/nba_api/stats/endpoints/playerfantasyprofile.py
--rw-r--r--   0        0        0     2271 2022-10-09 01:59:25.649190 nba_api-1.2/src/nba_api/stats/endpoints/playerfantasyprofilebargraph.py
--rw-r--r--   0        0        0     2199 2022-10-09 01:59:25.649190 nba_api-1.2/src/nba_api/stats/endpoints/playergamelog.py
--rw-r--r--   0        0        0     4645 2022-11-16 12:11:59.296582 nba_api-1.2/src/nba_api/stats/endpoints/playergamelogs.py
--rw-r--r--   0        0        0     9734 2022-10-09 01:59:25.650191 nba_api-1.2/src/nba_api/stats/endpoints/playergamestreakfinder.py
--rw-r--r--   0        0        0     3007 2023-03-23 21:23:27.982794 nba_api-1.2/src/nba_api/stats/endpoints/playerindex.py
--rw-r--r--   0        0        0     2151 2022-10-09 01:59:25.650191 nba_api-1.2/src/nba_api/stats/endpoints/playernextngames.py
--rw-r--r--   0        0        0     6830 2022-10-09 01:59:25.651187 nba_api-1.2/src/nba_api/stats/endpoints/playerprofilev2.py
--rw-r--r--   0        0        0     6494 2022-10-09 01:59:25.651187 nba_api-1.2/src/nba_api/stats/endpoints/playervsplayer.py
--rw-r--r--   0        0        0     5337 2022-10-09 01:59:25.651187 nba_api-1.2/src/nba_api/stats/endpoints/playoffpicture.py
--rw-r--r--   0        0        0     3623 2022-10-09 01:59:25.652191 nba_api-1.2/src/nba_api/stats/endpoints/scoreboard.py
--rw-r--r--   0        0        0     4244 2022-10-09 01:59:25.652191 nba_api-1.2/src/nba_api/stats/endpoints/scoreboardv2.py
--rw-r--r--   0        0        0     5617 2022-10-09 01:59:25.652191 nba_api-1.2/src/nba_api/stats/endpoints/shotchartdetail.py
--rw-r--r--   0        0        0     1635 2022-10-09 01:59:25.652191 nba_api-1.2/src/nba_api/stats/endpoints/shotchartleaguewide.py
--rw-r--r--   0        0        0     4288 2022-10-09 01:59:25.653190 nba_api-1.2/src/nba_api/stats/endpoints/shotchartlineupdetail.py
--rw-r--r--   0        0        0     2526 2022-10-09 01:59:25.653190 nba_api-1.2/src/nba_api/stats/endpoints/synergyplaytypes.py
--rw-r--r--   0        0        0     6624 2022-10-09 01:59:25.653190 nba_api-1.2/src/nba_api/stats/endpoints/teamandplayersvsplayers.py
--rw-r--r--   0        0        0    11922 2022-10-09 01:59:25.654186 nba_api-1.2/src/nba_api/stats/endpoints/teamdashboardbyclutch.py
--rw-r--r--   0        0        0     7440 2022-10-09 01:59:25.654186 nba_api-1.2/src/nba_api/stats/endpoints/teamdashboardbygamesplits.py
--rw-r--r--   0        0        0     8251 2022-10-09 01:59:25.654186 nba_api-1.2/src/nba_api/stats/endpoints/teamdashboardbygeneralsplits.py
--rw-r--r--   0        0        0     8090 2022-10-09 01:59:25.655187 nba_api-1.2/src/nba_api/stats/endpoints/teamdashboardbylastngames.py
--rw-r--r--   0        0        0     6706 2022-10-09 01:59:25.655187 nba_api-1.2/src/nba_api/stats/endpoints/teamdashboardbyopponent.py
--rw-r--r--   0        0        0     7870 2022-10-09 01:59:25.655187 nba_api-1.2/src/nba_api/stats/endpoints/teamdashboardbyshootingsplits.py
--rw-r--r--   0        0        0     6882 2022-10-09 01:59:25.656186 nba_api-1.2/src/nba_api/stats/endpoints/teamdashboardbyteamperformance.py
--rw-r--r--   0        0        0     5297 2022-10-09 01:59:25.656186 nba_api-1.2/src/nba_api/stats/endpoints/teamdashboardbyyearoveryear.py
--rw-r--r--   0        0        0     5414 2022-10-09 01:59:25.656186 nba_api-1.2/src/nba_api/stats/endpoints/teamdashlineups.py
--rw-r--r--   0        0        0     3465 2022-10-09 01:59:25.657188 nba_api-1.2/src/nba_api/stats/endpoints/teamdashptpass.py
--rw-r--r--   0        0        0     4669 2022-10-09 01:59:25.657188 nba_api-1.2/src/nba_api/stats/endpoints/teamdashptreb.py
--rw-r--r--   0        0        0     5081 2022-10-09 01:59:25.657188 nba_api-1.2/src/nba_api/stats/endpoints/teamdashptshots.py
--rw-r--r--   0        0        0     2567 2022-10-09 01:59:25.658189 nba_api-1.2/src/nba_api/stats/endpoints/teamdetails.py
--rw-r--r--   0        0        0     2097 2022-10-09 01:59:25.658189 nba_api-1.2/src/nba_api/stats/endpoints/teamestimatedmetrics.py
--rw-r--r--   0        0        0     2154 2022-10-09 01:59:25.659190 nba_api-1.2/src/nba_api/stats/endpoints/teamgamelog.py
--rw-r--r--   0        0        0     4533 2022-10-09 01:59:25.659190 nba_api-1.2/src/nba_api/stats/endpoints/teamgamelogs.py
--rw-r--r--   0        0        0    19511 2022-10-09 01:59:25.659190 nba_api-1.2/src/nba_api/stats/endpoints/teamgamestreakfinder.py
--rw-r--r--   0        0        0     1864 2022-10-09 01:59:25.660187 nba_api-1.2/src/nba_api/stats/endpoints/teamhistoricalleaders.py
--rw-r--r--   0        0        0     2330 2022-10-09 01:59:25.660187 nba_api-1.2/src/nba_api/stats/endpoints/teaminfocommon.py
--rw-r--r--   0        0        0     5330 2022-10-09 01:59:25.660187 nba_api-1.2/src/nba_api/stats/endpoints/teamplayerdashboard.py
--rw-r--r--   0        0        0     6024 2022-10-09 01:59:25.660187 nba_api-1.2/src/nba_api/stats/endpoints/teamplayeronoffdetails.py
--rw-r--r--   0        0        0     5102 2022-10-09 01:59:25.661187 nba_api-1.2/src/nba_api/stats/endpoints/teamplayeronoffsummary.py
--rw-r--r--   0        0        0     7583 2022-10-09 01:59:25.661187 nba_api-1.2/src/nba_api/stats/endpoints/teamvsplayer.py
--rw-r--r--   0        0        0     2103 2022-10-09 01:59:25.661187 nba_api-1.2/src/nba_api/stats/endpoints/teamyearbyyearstats.py
--rw-r--r--   0        0        0     4826 2022-10-09 01:59:25.662186 nba_api-1.2/src/nba_api/stats/endpoints/videodetails.py
--rw-r--r--   0        0        0     4834 2023-03-23 21:24:17.858394 nba_api-1.2/src/nba_api/stats/endpoints/videodetailsasset.py
--rw-r--r--   0        0        0     1357 2022-10-09 01:59:25.662186 nba_api-1.2/src/nba_api/stats/endpoints/videoevents.py
--rw-r--r--   0        0        0     1367 2022-10-09 01:59:25.662186 nba_api-1.2/src/nba_api/stats/endpoints/videoeventsasset.py
--rw-r--r--   0        0        0     1802 2022-10-09 01:59:25.663186 nba_api-1.2/src/nba_api/stats/endpoints/videostatus.py
--rw-r--r--   0        0        0     1943 2022-10-09 01:59:25.663186 nba_api-1.2/src/nba_api/stats/endpoints/winprobabilitypbp.py
--rw-r--r--   0        0        0        0 2022-10-09 01:59:25.663186 nba_api-1.2/src/nba_api/stats/library/__init__.py
--rw-r--r--   0        0        0   278496 2023-03-23 21:23:27.982794 nba_api-1.2/src/nba_api/stats/library/data.py
--rw-r--r--   0        0        0      334 2022-10-19 10:37:01.307007 nba_api-1.2/src/nba_api/stats/library/eventmsgtype.py
--rw-r--r--   0        0        0     3511 2022-10-09 01:59:25.666187 nba_api-1.2/src/nba_api/stats/library/http.py
--rw-r--r--   0        0        0    15350 2023-03-23 21:23:27.982794 nba_api-1.2/src/nba_api/stats/library/parameters.py
--rw-r--r--   0        0        0     4936 2022-10-19 10:37:01.307007 nba_api-1.2/src/nba_api/stats/library/playbyplayregex.py
--rw-r--r--   0        0        0       32 2022-10-09 01:59:25.667187 nba_api-1.2/src/nba_api/stats/static/__init__.py
--rw-r--r--   0        0        0     2059 2022-10-09 01:59:25.667187 nba_api-1.2/src/nba_api/stats/static/players.py
--rw-r--r--   0        0        0     2614 2022-10-09 01:59:25.668187 nba_api-1.2/src/nba_api/stats/static/teams.py
--rw-r--r--   0        0        0     5471 1970-01-01 00:00:00.000000 nba_api-1.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1088 2023-06-13 11:14:20.344592 nba_api-1.2.1/LICENSE
+-rwxr-xr-x   0        0        0     4419 2023-06-13 11:14:20.345485 nba_api-1.2.1/README.md
+-rwxr-xr-x   0        0        0     1161 2023-06-13 13:47:02.601749 nba_api-1.2.1/pyproject.toml
+-rwxr-xr-x   0        0        0       18 2023-06-13 11:14:20.407146 nba_api-1.2.1/src/nba_api/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-06-13 11:14:20.408145 nba_api-1.2.1/src/nba_api/library/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-06-13 11:14:20.408145 nba_api-1.2.1/src/nba_api/library/debug/__init__.py
+-rwxr-xr-x   0        0        0      192 2023-06-13 11:14:20.408145 nba_api-1.2.1/src/nba_api/library/debug/debug.py
+-rwxr-xr-x   0        0        0     4288 2023-06-13 11:14:20.408145 nba_api-1.2.1/src/nba_api/library/http.py
+-rwxr-xr-x   0        0        0        2 2023-06-13 11:14:20.409142 nba_api-1.2.1/src/nba_api/live/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-06-13 11:14:20.409142 nba_api-1.2.1/src/nba_api/live/nba/__init__.py
+-rwxr-xr-x   0        0        0      178 2023-06-13 11:14:20.410173 nba_api-1.2.1/src/nba_api/live/nba/endpoints/__init__.py
+-rwxr-xr-x   0        0        0      601 2023-06-13 11:14:20.410173 nba_api-1.2.1/src/nba_api/live/nba/endpoints/_base.py
+-rwxr-xr-x   0        0        0     9894 2023-06-13 11:14:20.410173 nba_api-1.2.1/src/nba_api/live/nba/endpoints/boxscore.py
+-rw-r--r--   0        0        0     2534 2023-06-13 13:25:33.292356 nba_api-1.2.1/src/nba_api/live/nba/endpoints/playbyplay.py
+-rwxr-xr-x   0        0        0     2484 2023-06-13 11:14:20.411145 nba_api-1.2.1/src/nba_api/live/nba/endpoints/scoreboard.py
+-rwxr-xr-x   0        0        0        0 2023-06-13 11:14:20.411145 nba_api-1.2.1/src/nba_api/live/nba/library/__init__.py
+-rwxr-xr-x   0        0        0     1043 2023-06-13 11:14:20.411145 nba_api-1.2.1/src/nba_api/live/nba/library/http.py
+-rwxr-xr-x   0        0        0        0 2023-06-13 11:14:20.412143 nba_api-1.2.1/src/nba_api/stats/__init__.py
+-rwxr-xr-x   0        0        0    10950 2023-06-13 11:14:20.412143 nba_api-1.2.1/src/nba_api/stats/endpoints/__init__.py
+-rwxr-xr-x   0        0        0     2275 2023-06-13 11:14:20.412143 nba_api-1.2.1/src/nba_api/stats/endpoints/_base.py
+-rwxr-xr-x   0        0        0     4331 2023-06-13 11:14:20.413143 nba_api-1.2.1/src/nba_api/stats/endpoints/alltimeleadersgrids.py
+-rwxr-xr-x   0        0        0     1956 2023-06-13 11:14:20.413143 nba_api-1.2.1/src/nba_api/stats/endpoints/assistleaders.py
+-rwxr-xr-x   0        0        0     4820 2023-06-13 11:14:20.413143 nba_api-1.2.1/src/nba_api/stats/endpoints/assisttracker.py
+-rwxr-xr-x   0        0        0     2771 2023-06-13 11:14:20.414143 nba_api-1.2.1/src/nba_api/stats/endpoints/boxscoreadvancedv2.py
+-rwxr-xr-x   0        0        0     1830 2023-06-13 11:14:20.414143 nba_api-1.2.1/src/nba_api/stats/endpoints/boxscoredefensive.py
+-rwxr-xr-x   0        0        0     2515 2023-06-13 11:14:20.414143 nba_api-1.2.1/src/nba_api/stats/endpoints/boxscorefourfactorsv2.py
+-rwxr-xr-x   0        0        0     2044 2023-06-13 11:14:20.415141 nba_api-1.2.1/src/nba_api/stats/endpoints/boxscorematchups.py
+-rwxr-xr-x   0        0        0     2547 2023-06-13 11:14:20.415141 nba_api-1.2.1/src/nba_api/stats/endpoints/boxscoremiscv2.py
+-rwxr-xr-x   0        0        0     2000 2023-06-13 11:14:20.415141 nba_api-1.2.1/src/nba_api/stats/endpoints/boxscoreplayertrackv2.py
+-rwxr-xr-x   0        0        0     2729 2023-06-13 11:14:20.415141 nba_api-1.2.1/src/nba_api/stats/endpoints/boxscorescoringv2.py
+-rwxr-xr-x   0        0        0     2335 2023-06-13 11:14:20.416141 nba_api-1.2.1/src/nba_api/stats/endpoints/boxscoresimilarityscore.py
+-rwxr-xr-x   0        0        0     3686 2023-06-13 11:14:20.416141 nba_api-1.2.1/src/nba_api/stats/endpoints/boxscoresummaryv2.py
+-rwxr-xr-x   0        0        0     2891 2023-06-13 11:14:20.416141 nba_api-1.2.1/src/nba_api/stats/endpoints/boxscoretraditionalv2.py
+-rwxr-xr-x   0        0        0     2647 2023-06-13 11:14:20.416141 nba_api-1.2.1/src/nba_api/stats/endpoints/boxscoreusagev2.py
+-rwxr-xr-x   0        0        0     1899 2023-06-13 11:14:20.416141 nba_api-1.2.1/src/nba_api/stats/endpoints/commonallplayers.py
+-rwxr-xr-x   0        0        0     2335 2023-06-13 11:14:20.417142 nba_api-1.2.1/src/nba_api/stats/endpoints/commonplayerinfo.py
+-rwxr-xr-x   0        0        0     1710 2023-06-13 11:14:20.417142 nba_api-1.2.1/src/nba_api/stats/endpoints/commonplayoffseries.py
+-rwxr-xr-x   0        0        0     1999 2023-06-13 11:14:20.418145 nba_api-1.2.1/src/nba_api/stats/endpoints/commonteamroster.py
+-rwxr-xr-x   0        0        0     1509 2023-06-13 11:14:20.418145 nba_api-1.2.1/src/nba_api/stats/endpoints/commonteamyears.py
+-rwxr-xr-x   0        0        0     2793 2023-06-13 11:14:20.418145 nba_api-1.2.1/src/nba_api/stats/endpoints/cumestatsplayer.py
+-rwxr-xr-x   0        0        0     2428 2023-06-13 11:14:20.419143 nba_api-1.2.1/src/nba_api/stats/endpoints/cumestatsplayergames.py
+-rwxr-xr-x   0        0        0     2850 2023-06-13 11:14:20.419143 nba_api-1.2.1/src/nba_api/stats/endpoints/cumestatsteam.py
+-rwxr-xr-x   0        0        0     2502 2023-06-13 11:14:20.419143 nba_api-1.2.1/src/nba_api/stats/endpoints/cumestatsteamgames.py
+-rwxr-xr-x   0        0        0     3591 2023-06-13 11:14:20.419143 nba_api-1.2.1/src/nba_api/stats/endpoints/defensehub.py
+-rwxr-xr-x   0        0        0     2315 2023-06-13 11:14:20.420142 nba_api-1.2.1/src/nba_api/stats/endpoints/draftboard.py
+-rwxr-xr-x   0        0        0     1784 2023-06-13 11:14:20.420142 nba_api-1.2.1/src/nba_api/stats/endpoints/draftcombinedrillresults.py
+-rwxr-xr-x   0        0        0     2461 2023-06-13 11:14:20.420142 nba_api-1.2.1/src/nba_api/stats/endpoints/draftcombinenonstationaryshooting.py
+-rwxr-xr-x   0        0        0     1860 2023-06-13 11:14:20.421143 nba_api-1.2.1/src/nba_api/stats/endpoints/draftcombineplayeranthro.py
+-rwxr-xr-x   0        0        0     2841 2023-06-13 11:14:20.421143 nba_api-1.2.1/src/nba_api/stats/endpoints/draftcombinespotshooting.py
+-rwxr-xr-x   0        0        0     2631 2023-06-13 11:14:20.421143 nba_api-1.2.1/src/nba_api/stats/endpoints/draftcombinestats.py
+-rwxr-xr-x   0        0        0     2304 2023-06-13 11:14:20.422143 nba_api-1.2.1/src/nba_api/stats/endpoints/drafthistory.py
+-rwxr-xr-x   0        0        0     3695 2023-06-13 11:14:20.422143 nba_api-1.2.1/src/nba_api/stats/endpoints/fantasywidget.py
+-rwxr-xr-x   0        0        0     1939 2023-06-13 11:14:20.422143 nba_api-1.2.1/src/nba_api/stats/endpoints/franchisehistory.py
+-rwxr-xr-x   0        0        0     1766 2023-06-13 11:14:20.423142 nba_api-1.2.1/src/nba_api/stats/endpoints/franchiseleaders.py
+-rwxr-xr-x   0        0        0     2029 2023-06-13 11:14:20.423142 nba_api-1.2.1/src/nba_api/stats/endpoints/franchiseplayers.py
+-rwxr-xr-x   0        0        0     1906 2023-06-13 11:14:20.423142 nba_api-1.2.1/src/nba_api/stats/endpoints/gamerotation.py
+-rwxr-xr-x   0        0        0     2374 2023-06-13 11:14:20.423142 nba_api-1.2.1/src/nba_api/stats/endpoints/glalumboxscoresimilarityscore.py
+-rwxr-xr-x   0        0        0     2609 2023-06-13 11:14:20.424022 nba_api-1.2.1/src/nba_api/stats/endpoints/homepageleaders.py
+-rwxr-xr-x   0        0        0     3313 2023-06-13 11:14:20.424022 nba_api-1.2.1/src/nba_api/stats/endpoints/homepagev2.py
+-rwxr-xr-x   0        0        0     2455 2023-06-13 11:14:20.424537 nba_api-1.2.1/src/nba_api/stats/endpoints/hustlestatsboxscore.py
+-rwxr-xr-x   0        0        0     1737 2023-06-13 11:14:20.424537 nba_api-1.2.1/src/nba_api/stats/endpoints/infographicfanduelplayer.py
+-rwxr-xr-x   0        0        0     2667 2023-06-13 11:14:20.424990 nba_api-1.2.1/src/nba_api/stats/endpoints/leaderstiles.py
+-rwxr-xr-x   0        0        0     4975 2023-06-13 11:14:20.424990 nba_api-1.2.1/src/nba_api/stats/endpoints/leaguedashlineups.py
+-rwxr-xr-x   0        0        0     4608 2023-06-13 11:14:20.425674 nba_api-1.2.1/src/nba_api/stats/endpoints/leaguedashoppptshot.py
+-rwxr-xr-x   0        0        0     5445 2023-06-13 11:14:20.425674 nba_api-1.2.1/src/nba_api/stats/endpoints/leaguedashplayerbiostats.py
+-rwxr-xr-x   0        0        0     6551 2023-06-13 11:14:20.426182 nba_api-1.2.1/src/nba_api/stats/endpoints/leaguedashplayerclutch.py
+-rwxr-xr-x   0        0        0     5660 2023-06-13 11:14:20.426716 nba_api-1.2.1/src/nba_api/stats/endpoints/leaguedashplayerptshot.py
+-rwxr-xr-x   0        0        0     6087 2023-06-13 11:14:20.427309 nba_api-1.2.1/src/nba_api/stats/endpoints/leaguedashplayershotlocations.py
+-rwxr-xr-x   0        0        0     6299 2023-06-13 11:14:20.427309 nba_api-1.2.1/src/nba_api/stats/endpoints/leaguedashplayerstats.py
+-rwxr-xr-x   0        0        0     5132 2023-06-13 11:14:20.427889 nba_api-1.2.1/src/nba_api/stats/endpoints/leaguedashptdefend.py
+-rwxr-xr-x   0        0        0     5061 2023-06-13 11:14:20.427889 nba_api-1.2.1/src/nba_api/stats/endpoints/leaguedashptstats.py
+-rwxr-xr-x   0        0        0     3988 2023-06-13 11:14:20.428396 nba_api-1.2.1/src/nba_api/stats/endpoints/leaguedashptteamdefend.py
+-rwxr-xr-x   0        0        0     5884 2023-06-13 11:14:20.428396 nba_api-1.2.1/src/nba_api/stats/endpoints/leaguedashteamclutch.py
+-rwxr-xr-x   0        0        0     4610 2023-06-13 11:14:20.428932 nba_api-1.2.1/src/nba_api/stats/endpoints/leaguedashteamptshot.py
+-rwxr-xr-x   0        0        0     5520 2023-06-13 11:14:20.429580 nba_api-1.2.1/src/nba_api/stats/endpoints/leaguedashteamshotlocations.py
+-rwxr-xr-x   0        0        0     5645 2023-06-13 11:14:20.429580 nba_api-1.2.1/src/nba_api/stats/endpoints/leaguedashteamstats.py
+-rwxr-xr-x   0        0        0     9785 2023-06-13 11:14:20.430086 nba_api-1.2.1/src/nba_api/stats/endpoints/leaguegamefinder.py
+-rwxr-xr-x   0        0        0     2545 2023-06-13 11:14:20.430160 nba_api-1.2.1/src/nba_api/stats/endpoints/leaguegamelog.py
+-rwxr-xr-x   0        0        0     4768 2023-06-13 11:14:20.430160 nba_api-1.2.1/src/nba_api/stats/endpoints/leaguehustlestatsplayer.py
+-rwxr-xr-x   0        0        0     5447 2023-06-13 11:14:20.430852 nba_api-1.2.1/src/nba_api/stats/endpoints/leaguehustlestatsplayerleaders.py
+-rwxr-xr-x   0        0        0     4614 2023-06-13 11:14:20.430852 nba_api-1.2.1/src/nba_api/stats/endpoints/leaguehustlestatsteam.py
+-rwxr-xr-x   0        0        0     5424 2023-06-13 11:14:20.431358 nba_api-1.2.1/src/nba_api/stats/endpoints/leaguehustlestatsteamleaders.py
+-rwxr-xr-x   0        0        0     2335 2023-06-13 11:14:20.431358 nba_api-1.2.1/src/nba_api/stats/endpoints/leagueleaders.py
+-rwxr-xr-x   0        0        0     4807 2023-06-13 11:14:20.431893 nba_api-1.2.1/src/nba_api/stats/endpoints/leaguelineupviz.py
+-rwxr-xr-x   0        0        0     4440 2023-06-13 11:14:20.431893 nba_api-1.2.1/src/nba_api/stats/endpoints/leagueplayerondetails.py
+-rwxr-xr-x   0        0        0     2572 2023-06-13 11:14:20.432513 nba_api-1.2.1/src/nba_api/stats/endpoints/leagueseasonmatchups.py
+-rwxr-xr-x   0        0        0     2914 2023-06-13 11:14:20.432513 nba_api-1.2.1/src/nba_api/stats/endpoints/leaguestandings.py
+-rwxr-xr-x   0        0        0     3788 2023-06-13 11:14:20.433019 nba_api-1.2.1/src/nba_api/stats/endpoints/leaguestandingsv3.py
+-rwxr-xr-x   0        0        0     2503 2023-06-13 11:14:20.433019 nba_api-1.2.1/src/nba_api/stats/endpoints/matchupsrollup.py
+-rwxr-xr-x   0        0        0     1935 2023-06-13 11:14:20.433019 nba_api-1.2.1/src/nba_api/stats/endpoints/playbyplay.py
+-rwxr-xr-x   0        0        0     2380 2023-06-13 11:14:20.434093 nba_api-1.2.1/src/nba_api/stats/endpoints/playbyplayv2.py
+-rwxr-xr-x   0        0        0     1547 2023-06-13 11:14:20.434746 nba_api-1.2.1/src/nba_api/stats/endpoints/playerawards.py
+-rwxr-xr-x   0        0        0     2123 2023-06-13 11:14:20.434834 nba_api-1.2.1/src/nba_api/stats/endpoints/playercareerbycollege.py
+-rwxr-xr-x   0        0        0     2822 2023-06-13 11:14:20.435422 nba_api-1.2.1/src/nba_api/stats/endpoints/playercareerbycollegerollup.py
+-rwxr-xr-x   0        0        0     5370 2023-06-13 11:14:20.435422 nba_api-1.2.1/src/nba_api/stats/endpoints/playercareerstats.py
+-rwxr-xr-x   0        0        0     4752 2023-06-13 11:14:20.436046 nba_api-1.2.1/src/nba_api/stats/endpoints/playercompare.py
+-rwxr-xr-x   0        0        0    12845 2023-06-13 11:14:20.436553 nba_api-1.2.1/src/nba_api/stats/endpoints/playerdashboardbyclutch.py
+-rwxr-xr-x   0        0        0     7841 2023-06-13 11:14:20.437104 nba_api-1.2.1/src/nba_api/stats/endpoints/playerdashboardbygamesplits.py
+-rwxr-xr-x   0        0        0     9392 2023-06-13 11:14:20.437104 nba_api-1.2.1/src/nba_api/stats/endpoints/playerdashboardbygeneralsplits.py
+-rwxr-xr-x   0        0        0     8578 2023-06-13 11:14:20.437104 nba_api-1.2.1/src/nba_api/stats/endpoints/playerdashboardbylastngames.py
+-rwxr-xr-x   0        0        0     7020 2023-06-13 11:14:20.438123 nba_api-1.2.1/src/nba_api/stats/endpoints/playerdashboardbyopponent.py
+-rwxr-xr-x   0        0        0     8237 2023-06-13 11:14:20.438123 nba_api-1.2.1/src/nba_api/stats/endpoints/playerdashboardbyshootingsplits.py
+-rwxr-xr-x   0        0        0     7196 2023-06-13 11:14:20.438123 nba_api-1.2.1/src/nba_api/stats/endpoints/playerdashboardbyteamperformance.py
+-rwxr-xr-x   0        0        0     5535 2023-06-13 11:14:20.438123 nba_api-1.2.1/src/nba_api/stats/endpoints/playerdashboardbyyearoveryear.py
+-rwxr-xr-x   0        0        0     3658 2023-06-13 11:14:20.439118 nba_api-1.2.1/src/nba_api/stats/endpoints/playerdashptpass.py
+-rwxr-xr-x   0        0        0     4817 2023-06-13 11:14:20.439118 nba_api-1.2.1/src/nba_api/stats/endpoints/playerdashptreb.py
+-rwxr-xr-x   0        0        0     3440 2023-06-13 11:14:20.439118 nba_api-1.2.1/src/nba_api/stats/endpoints/playerdashptshotdefend.py
+-rwxr-xr-x   0        0        0     5580 2023-06-13 11:14:20.440125 nba_api-1.2.1/src/nba_api/stats/endpoints/playerdashptshots.py
+-rwxr-xr-x   0        0        0     2136 2023-06-13 11:14:20.440125 nba_api-1.2.1/src/nba_api/stats/endpoints/playerestimatedmetrics.py
+-rwxr-xr-x   0        0        0     4068 2023-06-13 11:14:20.440125 nba_api-1.2.1/src/nba_api/stats/endpoints/playerfantasyprofile.py
+-rwxr-xr-x   0        0        0     2271 2023-06-13 11:14:20.440125 nba_api-1.2.1/src/nba_api/stats/endpoints/playerfantasyprofilebargraph.py
+-rwxr-xr-x   0        0        0     2199 2023-06-13 11:14:20.441116 nba_api-1.2.1/src/nba_api/stats/endpoints/playergamelog.py
+-rwxr-xr-x   0        0        0     4645 2023-06-13 11:14:20.441116 nba_api-1.2.1/src/nba_api/stats/endpoints/playergamelogs.py
+-rwxr-xr-x   0        0        0     9734 2023-06-13 11:14:20.442116 nba_api-1.2.1/src/nba_api/stats/endpoints/playergamestreakfinder.py
+-rwxr-xr-x   0        0        0     3008 2023-06-13 11:14:20.442116 nba_api-1.2.1/src/nba_api/stats/endpoints/playerindex.py
+-rwxr-xr-x   0        0        0     2151 2023-06-13 11:14:20.443116 nba_api-1.2.1/src/nba_api/stats/endpoints/playernextngames.py
+-rwxr-xr-x   0        0        0     6830 2023-06-13 11:14:20.443116 nba_api-1.2.1/src/nba_api/stats/endpoints/playerprofilev2.py
+-rwxr-xr-x   0        0        0     6494 2023-06-13 11:14:20.443116 nba_api-1.2.1/src/nba_api/stats/endpoints/playervsplayer.py
+-rwxr-xr-x   0        0        0     5337 2023-06-13 11:14:20.443116 nba_api-1.2.1/src/nba_api/stats/endpoints/playoffpicture.py
+-rwxr-xr-x   0        0        0     3623 2023-06-13 11:14:20.444116 nba_api-1.2.1/src/nba_api/stats/endpoints/scoreboard.py
+-rwxr-xr-x   0        0        0     4244 2023-06-13 11:14:20.444116 nba_api-1.2.1/src/nba_api/stats/endpoints/scoreboardv2.py
+-rwxr-xr-x   0        0        0     5617 2023-06-13 11:14:20.444116 nba_api-1.2.1/src/nba_api/stats/endpoints/shotchartdetail.py
+-rwxr-xr-x   0        0        0     1635 2023-06-13 11:14:20.444116 nba_api-1.2.1/src/nba_api/stats/endpoints/shotchartleaguewide.py
+-rwxr-xr-x   0        0        0     4288 2023-06-13 11:14:20.445115 nba_api-1.2.1/src/nba_api/stats/endpoints/shotchartlineupdetail.py
+-rwxr-xr-x   0        0        0     2526 2023-06-13 11:14:20.445115 nba_api-1.2.1/src/nba_api/stats/endpoints/synergyplaytypes.py
+-rwxr-xr-x   0        0        0     6624 2023-06-13 11:14:20.445115 nba_api-1.2.1/src/nba_api/stats/endpoints/teamandplayersvsplayers.py
+-rwxr-xr-x   0        0        0    11922 2023-06-13 11:14:20.446115 nba_api-1.2.1/src/nba_api/stats/endpoints/teamdashboardbyclutch.py
+-rwxr-xr-x   0        0        0     7440 2023-06-13 11:14:20.446115 nba_api-1.2.1/src/nba_api/stats/endpoints/teamdashboardbygamesplits.py
+-rwxr-xr-x   0        0        0     8251 2023-06-13 11:14:20.446115 nba_api-1.2.1/src/nba_api/stats/endpoints/teamdashboardbygeneralsplits.py
+-rwxr-xr-x   0        0        0     8090 2023-06-13 11:14:20.447113 nba_api-1.2.1/src/nba_api/stats/endpoints/teamdashboardbylastngames.py
+-rwxr-xr-x   0        0        0     6706 2023-06-13 11:14:20.447113 nba_api-1.2.1/src/nba_api/stats/endpoints/teamdashboardbyopponent.py
+-rwxr-xr-x   0        0        0     7870 2023-06-13 11:14:20.447113 nba_api-1.2.1/src/nba_api/stats/endpoints/teamdashboardbyshootingsplits.py
+-rwxr-xr-x   0        0        0     6882 2023-06-13 11:14:20.447113 nba_api-1.2.1/src/nba_api/stats/endpoints/teamdashboardbyteamperformance.py
+-rwxr-xr-x   0        0        0     5297 2023-06-13 11:14:20.448119 nba_api-1.2.1/src/nba_api/stats/endpoints/teamdashboardbyyearoveryear.py
+-rwxr-xr-x   0        0        0     5414 2023-06-13 11:14:20.448119 nba_api-1.2.1/src/nba_api/stats/endpoints/teamdashlineups.py
+-rwxr-xr-x   0        0        0     3465 2023-06-13 11:14:20.448119 nba_api-1.2.1/src/nba_api/stats/endpoints/teamdashptpass.py
+-rwxr-xr-x   0        0        0     4669 2023-06-13 11:14:20.448119 nba_api-1.2.1/src/nba_api/stats/endpoints/teamdashptreb.py
+-rwxr-xr-x   0        0        0     5081 2023-06-13 11:14:20.449115 nba_api-1.2.1/src/nba_api/stats/endpoints/teamdashptshots.py
+-rwxr-xr-x   0        0        0     2567 2023-06-13 11:14:20.449115 nba_api-1.2.1/src/nba_api/stats/endpoints/teamdetails.py
+-rwxr-xr-x   0        0        0     2097 2023-06-13 11:14:20.449115 nba_api-1.2.1/src/nba_api/stats/endpoints/teamestimatedmetrics.py
+-rwxr-xr-x   0        0        0     2154 2023-06-13 11:14:20.450140 nba_api-1.2.1/src/nba_api/stats/endpoints/teamgamelog.py
+-rwxr-xr-x   0        0        0     4533 2023-06-13 11:14:20.450140 nba_api-1.2.1/src/nba_api/stats/endpoints/teamgamelogs.py
+-rwxr-xr-x   0        0        0    19511 2023-06-13 11:14:20.450140 nba_api-1.2.1/src/nba_api/stats/endpoints/teamgamestreakfinder.py
+-rwxr-xr-x   0        0        0     1864 2023-06-13 11:14:20.450140 nba_api-1.2.1/src/nba_api/stats/endpoints/teamhistoricalleaders.py
+-rwxr-xr-x   0        0        0     2330 2023-06-13 11:14:20.451136 nba_api-1.2.1/src/nba_api/stats/endpoints/teaminfocommon.py
+-rwxr-xr-x   0        0        0     5330 2023-06-13 11:14:20.451136 nba_api-1.2.1/src/nba_api/stats/endpoints/teamplayerdashboard.py
+-rwxr-xr-x   0        0        0     6024 2023-06-13 11:14:20.452204 nba_api-1.2.1/src/nba_api/stats/endpoints/teamplayeronoffdetails.py
+-rwxr-xr-x   0        0        0     5102 2023-06-13 11:14:20.452204 nba_api-1.2.1/src/nba_api/stats/endpoints/teamplayeronoffsummary.py
+-rwxr-xr-x   0        0        0     7583 2023-06-13 11:14:20.452204 nba_api-1.2.1/src/nba_api/stats/endpoints/teamvsplayer.py
+-rwxr-xr-x   0        0        0     2103 2023-06-13 11:14:20.452204 nba_api-1.2.1/src/nba_api/stats/endpoints/teamyearbyyearstats.py
+-rwxr-xr-x   0        0        0     4826 2023-06-13 11:14:20.453215 nba_api-1.2.1/src/nba_api/stats/endpoints/videodetails.py
+-rwxr-xr-x   0        0        0     4834 2023-06-13 11:14:20.453215 nba_api-1.2.1/src/nba_api/stats/endpoints/videodetailsasset.py
+-rwxr-xr-x   0        0        0     1357 2023-06-13 11:14:20.453215 nba_api-1.2.1/src/nba_api/stats/endpoints/videoevents.py
+-rwxr-xr-x   0        0        0     1367 2023-06-13 11:14:20.454214 nba_api-1.2.1/src/nba_api/stats/endpoints/videoeventsasset.py
+-rwxr-xr-x   0        0        0     1802 2023-06-13 11:14:20.454214 nba_api-1.2.1/src/nba_api/stats/endpoints/videostatus.py
+-rwxr-xr-x   0        0        0     1943 2023-06-13 11:14:20.454214 nba_api-1.2.1/src/nba_api/stats/endpoints/winprobabilitypbp.py
+-rwxr-xr-x   0        0        0        0 2023-06-13 11:14:20.454214 nba_api-1.2.1/src/nba_api/stats/library/__init__.py
+-rwxr-xr-x   0        0        0   278496 2023-06-13 11:14:20.457214 nba_api-1.2.1/src/nba_api/stats/library/data.py
+-rwxr-xr-x   0        0        0      334 2023-06-13 11:14:20.457214 nba_api-1.2.1/src/nba_api/stats/library/eventmsgtype.py
+-rwxr-xr-x   0        0        0     3511 2023-06-13 11:14:20.458215 nba_api-1.2.1/src/nba_api/stats/library/http.py
+-rwxr-xr-x   0        0        0    15350 2023-06-13 11:14:20.458215 nba_api-1.2.1/src/nba_api/stats/library/parameters.py
+-rwxr-xr-x   0        0        0     4936 2023-06-13 11:14:20.458215 nba_api-1.2.1/src/nba_api/stats/library/playbyplayregex.py
+-rwxr-xr-x   0        0        0       32 2023-06-13 11:14:20.459215 nba_api-1.2.1/src/nba_api/stats/static/__init__.py
+-rwxr-xr-x   0        0        0     2059 2023-06-13 11:14:20.459215 nba_api-1.2.1/src/nba_api/stats/static/players.py
+-rwxr-xr-x   0        0        0     2614 2023-06-13 11:14:20.459215 nba_api-1.2.1/src/nba_api/stats/static/teams.py
+-rw-r--r--   0        0        0     5472 1970-01-01 00:00:00.000000 nba_api-1.2.1/PKG-INFO
```

### Comparing `nba_api-1.2/LICENSE` & `nba_api-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/pyproject.toml` & `nba_api-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "nba_api"
-version = "1.2"
+version = "1.2.1"
 description = "An API Client package to access the APIs for NBA.com"
 license = "MIT"
 authors = [ 
      "Swar Patel <swar.m.patel@gmail.com>",
 ]
 maintainers = [
     "Swar Patel <swar.m.patel@gmail.com>",
```

### Comparing `nba_api-1.2/README.md` & `nba_api-1.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -184,94 +184,94 @@
 00000b70: 692f 7374 6174 732f 7374 6174 6963 2f74  i/stats/static/t
 00000b80: 6561 6d73 2e6d 6429 0d0a 0d0a 2320 4a6f  eams.md)....# Jo
 00000b90: 696e 2074 6865 2043 6f6d 6d75 6e69 7479  in the Community
 00000ba0: 0d0a 2323 2053 6c61 636b 0d0a 0d0a 4a6f  ..## Slack....Jo
 00000bb0: 696e 205b 536c 6163 6b5d 2868 7474 7073  in [Slack](https
 00000bc0: 3a2f 2f6a 6f69 6e2e 736c 6163 6b2e 636f  ://join.slack.co
 00000bd0: 6d2f 742f 6e62 6161 7069 2f73 6861 7265  m/t/nbaapi/share
-00000be0: 645f 696e 7669 7465 2f7a 742d 3169 7073  d_invite/zt-1ips
-00000bf0: 7561 6939 6a2d 476a 5a6a 7550 3953 327e  uai9j-GjZjuP9S2~
-00000c00: 5563 7a75 6e79 3174 3734 7a41 2920 746f  Uczuny1t74zA) to
-00000c10: 2067 6574 2068 656c 702c 2068 656c 7020   get help, help 
-00000c20: 6f74 6865 7273 2c20 7072 6f76 6964 6520  others, provide 
-00000c30: 6665 6564 6261 636b 2c20 7365 6520 616d  feedback, see am
-00000c40: 617a 696e 6720 7072 6f6a 6563 7473 2c20  azing projects, 
-00000c50: 7061 7274 6963 6970 6174 6573 2069 6e20  participates in 
-00000c60: 6469 7363 7573 7369 6f6e 732c 2061 6e64  discussions, and
-00000c70: 2063 6f6c 6c61 626f 7261 7465 2077 6974   collaborate wit
-00000c80: 6820 6f74 6865 7273 2066 726f 6d20 6172  h others from ar
-00000c90: 6f75 6e64 2074 6865 2077 6f72 6c64 2e0d  ound the world..
-00000ca0: 0a0d 0a23 2320 5374 6163 6b20 4f76 6572  ...## Stack Over
-00000cb0: 666c 6f77 0d0a 0d0a 4e6f 7420 6120 536c  flow....Not a Sl
-00000cc0: 6163 6b20 6661 6e3f 204e 6f20 7072 6f62  ack fan? No prob
-00000cd0: 6c65 6d2e 2048 6561 6420 6f76 6572 2074  lem. Head over t
-00000ce0: 6f20 5b53 7461 636b 4f76 6572 666c 6f77  o [StackOverflow
-00000cf0: 5d28 6874 7470 733a 2f2f 7374 6163 6b6f  ](https://stacko
-00000d00: 7665 7266 6c6f 772e 636f 6d2f 7175 6573  verflow.com/ques
-00000d10: 7469 6f6e 732f 7461 6767 6564 2f6e 6261  tions/tagged/nba
-00000d20: 2d61 7069 292e 2042 6520 7375 7265 2074  -api). Be sure t
-00000d30: 6f20 7461 6720 796f 7572 2070 6f73 7420  o tag your post 
-00000d40: 7769 7468 2060 6e62 612d 6170 6960 2e0d  with `nba-api`..
-00000d50: 0a0d 0a23 2043 6f6e 7472 6962 7574 696e  ...# Contributin
-00000d60: 670d 0a0d 0a2a 5365 6520 5b43 6f6e 7472  g....*See [Contr
-00000d70: 6962 7574 696e 6720 746f 2074 6865 204e  ibuting to the N
-00000d80: 4241 5f41 5049 5d28 6874 7470 733a 2f2f  BA_API](https://
-00000d90: 6769 7468 7562 2e63 6f6d 2f73 7761 722f  github.com/swar/
-00000da0: 6e62 615f 6170 692f 626c 6f62 2f6d 6173  nba_api/blob/mas
-00000db0: 7465 722f 434f 4e54 5249 4255 5449 4e47  ter/CONTRIBUTING
-00000dc0: 2e6d 6429 2066 6f72 2063 6f6d 706c 6574  .md) for complet
-00000dd0: 6520 6465 7461 696c 732e 2a0d 0a0d 0a23  e details.*....#
-00000de0: 2320 456e 6470 6f69 6e74 730d 0a0d 0a41  # Endpoints....A
-00000df0: 2073 6967 6e69 6669 6361 6e74 2070 7572   significant pur
-00000e00: 706f 7365 206f 6620 7468 6973 2070 6163  pose of this pac
-00000e10: 6b61 6765 2069 7320 746f 2063 6f6e 7469  kage is to conti
-00000e20: 6e75 6f75 736c 7920 6d61 7020 616e 6420  nuously map and 
-00000e30: 616e 616c 797a 6520 6173 206d 616e 7920  analyze as many 
-00000e40: 656e 6470 6f69 6e74 7320 6f6e 204e 4241  endpoints on NBA
-00000e50: 2e63 6f6d 2061 7320 706f 7373 6962 6c65  .com as possible
-00000e60: 2e20 5468 6520 646f 6375 6d65 6e74 6174  . The documentat
-00000e70: 696f 6e20 616e 6420 616e 616c 7973 6973  ion and analysis
-00000e80: 206f 6620 7468 6520 656e 6470 6f69 6e74   of the endpoint
-00000e90: 7320 616e 6420 7061 7261 6d65 7465 7273  s and parameters
-00000ea0: 2069 6e20 7468 6973 2070 6163 6b61 6765   in this package
-00000eb0: 2061 7265 2073 6f6d 6520 6f66 2074 6865   are some of the
-00000ec0: 206d 6f73 7420 6578 7465 6e73 6976 6520   most extensive 
-00000ed0: 696e 666f 726d 6174 696f 6e20 6176 6169  information avai
-00000ee0: 6c61 626c 652e 2041 7420 7468 6520 7361  lable. At the sa
-00000ef0: 6d65 2074 696d 652c 204e 4241 2e63 6f6d  me time, NBA.com
-00000f00: 2064 6f65 7320 6e6f 7420 7072 6f76 6964   does not provid
-00000f10: 6520 696e 666f 726d 6174 696f 6e20 7265  e information re
-00000f20: 6761 7264 696e 6720 6e65 772c 2063 6861  garding new, cha
-00000f30: 6e67 6564 2c20 6f72 2072 656d 6f76 6564  nged, or removed
-00000f40: 2065 6e64 706f 696e 7473 2e0d 0a0d 0a49   endpoints.....I
-00000f50: 6620 796f 7520 6669 6e64 2061 206e 6577  f you find a new
-00000f60: 2c20 6368 616e 6765 642c 206f 7220 6465  , changed, or de
-00000f70: 7072 6563 6174 6564 2065 6e64 706f 696e  precated endpoin
-00000f80: 742c 206f 7065 6e20 6120 5b47 6974 4875  t, open a [GitHu
-00000f90: 6220 4973 7375 655d 2868 7474 7073 3a2f  b Issue](https:/
-00000fa0: 2f67 6974 6875 622e 636f 6d2f 7377 6172  /github.com/swar
-00000fb0: 2f6e 6261 5f61 7069 2f69 7373 7565 7329  /nba_api/issues)
-00000fc0: 0d0a 0d0a 2323 2042 7567 730d 0a0d 0a45  ....## Bugs....E
-00000fd0: 6e63 6f75 6e74 6572 2061 2062 7567 2c20  ncounter a bug, 
-00000fe0: 5b72 6570 6f72 7420 6120 6275 675d 2868  [report a bug](h
-00000ff0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001000: 6d2f 7377 6172 2f6e 6261 5f61 7069 2f69  m/swar/nba_api/i
-00001010: 7373 7565 7329 2e0d 0a0d 0a23 204c 6963  ssues).....# Lic
-00001020: 656e 7365 2026 2054 6572 6d73 206f 6620  ense & Terms of 
-00001030: 5573 650d 0a0d 0a23 2320 4150 4920 436c  Use....## API Cl
-00001040: 6965 6e74 2050 6163 6b61 6765 0d0a 0d0a  ient Package....
-00001050: 5468 6520 606e 6261 5f61 7069 6020 7061  The `nba_api` pa
-00001060: 636b 6167 6520 6973 204f 7065 6e20 536f  ckage is Open So
-00001070: 7572 6365 2077 6974 6820 616e 205b 4d49  urce with an [MI
-00001080: 5420 4c69 6365 6e73 655d 2868 7474 7073  T License](https
-00001090: 3a2f 2f67 6974 6875 622e 636f 6d2f 7377  ://github.com/sw
-000010a0: 6172 2f6e 6261 5f61 7069 2f62 6c6f 622f  ar/nba_api/blob/
-000010b0: 6d61 7374 6572 2f4c 4943 454e 5345 292e  master/LICENSE).
-000010c0: 0d0a 0d0a 2323 204e 4241 2e63 6f6d 0d0a  ....## NBA.com..
-000010d0: 0d0a 4e42 412e 636f 6d20 6861 7320 6120  ..NBA.com has a 
-000010e0: 5b54 6572 6d73 206f 6620 5573 655d 2868  [Terms of Use](h
-000010f0: 7474 7073 3a2f 2f77 7777 2e6e 6261 2e63  ttps://www.nba.c
-00001100: 6f6d 2f74 6572 6d73 6f66 7573 6529 2072  om/termsofuse) r
-00001110: 6567 6172 6469 6e67 2074 6865 2075 7365  egarding the use
-00001120: 206f 6620 7468 6520 4e42 41e2 8099 7320   of the NBA...s 
-00001130: 6469 6769 7461 6c20 706c 6174 666f 726d  digital platform
-00001140: 732e 0d0a                                s...
+00000be0: 645f 696e 7669 7465 2f7a 742d 6361 7966  d_invite/zt-cayf
+00000bf0: 726e 666f 2d73 3972 7953 416d 4258 7842  rnfo-s9rySAmBXxB
+00000c00: 6c6f 4c30 3953 364e 304b 4129 2074 6f20  loL09S6N0KA) to 
+00000c10: 6765 7420 6865 6c70 2c20 6865 6c70 206f  get help, help o
+00000c20: 7468 6572 732c 2070 726f 7669 6465 2066  thers, provide f
+00000c30: 6565 6462 6163 6b2c 2073 6565 2061 6d61  eedback, see ama
+00000c40: 7a69 6e67 2070 726f 6a65 6374 732c 2070  zing projects, p
+00000c50: 6172 7469 6369 7061 7465 7320 696e 2064  articipates in d
+00000c60: 6973 6375 7373 696f 6e73 2c20 616e 6420  iscussions, and 
+00000c70: 636f 6c6c 6162 6f72 6174 6520 7769 7468  collaborate with
+00000c80: 206f 7468 6572 7320 6672 6f6d 2061 726f   others from aro
+00000c90: 756e 6420 7468 6520 776f 726c 642e 0d0a  und the world...
+00000ca0: 0d0a 2323 2053 7461 636b 204f 7665 7266  ..## Stack Overf
+00000cb0: 6c6f 770d 0a0d 0a4e 6f74 2061 2053 6c61  low....Not a Sla
+00000cc0: 636b 2066 616e 3f20 4e6f 2070 726f 626c  ck fan? No probl
+00000cd0: 656d 2e20 4865 6164 206f 7665 7220 746f  em. Head over to
+00000ce0: 205b 5374 6163 6b4f 7665 7266 6c6f 775d   [StackOverflow]
+00000cf0: 2868 7474 7073 3a2f 2f73 7461 636b 6f76  (https://stackov
+00000d00: 6572 666c 6f77 2e63 6f6d 2f71 7565 7374  erflow.com/quest
+00000d10: 696f 6e73 2f74 6167 6765 642f 6e62 612d  ions/tagged/nba-
+00000d20: 6170 6929 2e20 4265 2073 7572 6520 746f  api). Be sure to
+00000d30: 2074 6167 2079 6f75 7220 706f 7374 2077   tag your post w
+00000d40: 6974 6820 606e 6261 2d61 7069 602e 0d0a  ith `nba-api`...
+00000d50: 0d0a 2320 436f 6e74 7269 6275 7469 6e67  ..# Contributing
+00000d60: 0d0a 0d0a 2a53 6565 205b 436f 6e74 7269  ....*See [Contri
+00000d70: 6275 7469 6e67 2074 6f20 7468 6520 4e42  buting to the NB
+00000d80: 415f 4150 495d 2868 7474 7073 3a2f 2f67  A_API](https://g
+00000d90: 6974 6875 622e 636f 6d2f 7377 6172 2f6e  ithub.com/swar/n
+00000da0: 6261 5f61 7069 2f62 6c6f 622f 6d61 7374  ba_api/blob/mast
+00000db0: 6572 2f43 4f4e 5452 4942 5554 494e 472e  er/CONTRIBUTING.
+00000dc0: 6d64 2920 666f 7220 636f 6d70 6c65 7465  md) for complete
+00000dd0: 2064 6574 6169 6c73 2e2a 0d0a 0d0a 2323   details.*....##
+00000de0: 2045 6e64 706f 696e 7473 0d0a 0d0a 4120   Endpoints....A 
+00000df0: 7369 676e 6966 6963 616e 7420 7075 7270  significant purp
+00000e00: 6f73 6520 6f66 2074 6869 7320 7061 636b  ose of this pack
+00000e10: 6167 6520 6973 2074 6f20 636f 6e74 696e  age is to contin
+00000e20: 756f 7573 6c79 206d 6170 2061 6e64 2061  uously map and a
+00000e30: 6e61 6c79 7a65 2061 7320 6d61 6e79 2065  nalyze as many e
+00000e40: 6e64 706f 696e 7473 206f 6e20 4e42 412e  ndpoints on NBA.
+00000e50: 636f 6d20 6173 2070 6f73 7369 626c 652e  com as possible.
+00000e60: 2054 6865 2064 6f63 756d 656e 7461 7469   The documentati
+00000e70: 6f6e 2061 6e64 2061 6e61 6c79 7369 7320  on and analysis 
+00000e80: 6f66 2074 6865 2065 6e64 706f 696e 7473  of the endpoints
+00000e90: 2061 6e64 2070 6172 616d 6574 6572 7320   and parameters 
+00000ea0: 696e 2074 6869 7320 7061 636b 6167 6520  in this package 
+00000eb0: 6172 6520 736f 6d65 206f 6620 7468 6520  are some of the 
+00000ec0: 6d6f 7374 2065 7874 656e 7369 7665 2069  most extensive i
+00000ed0: 6e66 6f72 6d61 7469 6f6e 2061 7661 696c  nformation avail
+00000ee0: 6162 6c65 2e20 4174 2074 6865 2073 616d  able. At the sam
+00000ef0: 6520 7469 6d65 2c20 4e42 412e 636f 6d20  e time, NBA.com 
+00000f00: 646f 6573 206e 6f74 2070 726f 7669 6465  does not provide
+00000f10: 2069 6e66 6f72 6d61 7469 6f6e 2072 6567   information reg
+00000f20: 6172 6469 6e67 206e 6577 2c20 6368 616e  arding new, chan
+00000f30: 6765 642c 206f 7220 7265 6d6f 7665 6420  ged, or removed 
+00000f40: 656e 6470 6f69 6e74 732e 0d0a 0d0a 4966  endpoints.....If
+00000f50: 2079 6f75 2066 696e 6420 6120 6e65 772c   you find a new,
+00000f60: 2063 6861 6e67 6564 2c20 6f72 2064 6570   changed, or dep
+00000f70: 7265 6361 7465 6420 656e 6470 6f69 6e74  recated endpoint
+00000f80: 2c20 6f70 656e 2061 205b 4769 7448 7562  , open a [GitHub
+00000f90: 2049 7373 7565 5d28 6874 7470 733a 2f2f   Issue](https://
+00000fa0: 6769 7468 7562 2e63 6f6d 2f73 7761 722f  github.com/swar/
+00000fb0: 6e62 615f 6170 692f 6973 7375 6573 290d  nba_api/issues).
+00000fc0: 0a0d 0a23 2320 4275 6773 0d0a 0d0a 456e  ...## Bugs....En
+00000fd0: 636f 756e 7465 7220 6120 6275 672c 205b  counter a bug, [
+00000fe0: 7265 706f 7274 2061 2062 7567 5d28 6874  report a bug](ht
+00000ff0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001000: 2f73 7761 722f 6e62 615f 6170 692f 6973  /swar/nba_api/is
+00001010: 7375 6573 292e 0d0a 0d0a 2320 4c69 6365  sues).....# Lice
+00001020: 6e73 6520 2620 5465 726d 7320 6f66 2055  nse & Terms of U
+00001030: 7365 0d0a 0d0a 2323 2041 5049 2043 6c69  se....## API Cli
+00001040: 656e 7420 5061 636b 6167 650d 0a0d 0a54  ent Package....T
+00001050: 6865 2060 6e62 615f 6170 6960 2070 6163  he `nba_api` pac
+00001060: 6b61 6765 2069 7320 4f70 656e 2053 6f75  kage is Open Sou
+00001070: 7263 6520 7769 7468 2061 6e20 5b4d 4954  rce with an [MIT
+00001080: 204c 6963 656e 7365 5d28 6874 7470 733a   License](https:
+00001090: 2f2f 6769 7468 7562 2e63 6f6d 2f73 7761  //github.com/swa
+000010a0: 722f 6e62 615f 6170 692f 626c 6f62 2f6d  r/nba_api/blob/m
+000010b0: 6173 7465 722f 4c49 4345 4e53 4529 2e0d  aster/LICENSE)..
+000010c0: 0a0d 0a23 2320 4e42 412e 636f 6d0d 0a0d  ...## NBA.com...
+000010d0: 0a4e 4241 2e63 6f6d 2068 6173 2061 205b  .NBA.com has a [
+000010e0: 5465 726d 7320 6f66 2055 7365 5d28 6874  Terms of Use](ht
+000010f0: 7470 733a 2f2f 7777 772e 6e62 612e 636f  tps://www.nba.co
+00001100: 6d2f 7465 726d 736f 6675 7365 2920 7265  m/termsofuse) re
+00001110: 6761 7264 696e 6720 7468 6520 7573 6520  garding the use 
+00001120: 6f66 2074 6865 204e 4241 e280 9973 2064  of the NBA...s d
+00001130: 6967 6974 616c 2070 6c61 7466 6f72 6d73  igital platforms
+00001140: 2e0d 0a                                  ...
```

### Comparing `nba_api-1.2/src/nba_api/library/http.py` & `nba_api-1.2.1/src/nba_api/library/http.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/live/nba/endpoints/_base.py` & `nba_api-1.2.1/src/nba_api/live/nba/endpoints/_base.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/live/nba/endpoints/boxscore.py` & `nba_api-1.2.1/src/nba_api/live/nba/endpoints/boxscore.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/live/nba/endpoints/playbyplay.py` & `nba_api-1.2.1/src/nba_api/live/nba/endpoints/playbyplay.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/live/nba/endpoints/scoreboard.py` & `nba_api-1.2.1/src/nba_api/live/nba/endpoints/scoreboard.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/live/nba/library/http.py` & `nba_api-1.2.1/src/nba_api/live/nba/library/http.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/__init__.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/_base.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/_base.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/alltimeleadersgrids.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/alltimeleadersgrids.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/assistleaders.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/assistleaders.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/assisttracker.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/assisttracker.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/boxscoreadvancedv2.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/boxscoreadvancedv2.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/boxscoredefensive.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/boxscoredefensive.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/boxscorefourfactorsv2.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/boxscorefourfactorsv2.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/boxscorematchups.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/boxscorematchups.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/boxscoremiscv2.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/boxscoremiscv2.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/boxscoreplayertrackv2.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/boxscoreplayertrackv2.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/boxscorescoringv2.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/boxscorescoringv2.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/boxscoresimilarityscore.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/boxscoresimilarityscore.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/boxscoresummaryv2.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/boxscoresummaryv2.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/boxscoretraditionalv2.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/boxscoretraditionalv2.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/boxscoreusagev2.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/boxscoreusagev2.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/commonallplayers.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/commonallplayers.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/commonplayerinfo.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/commonplayerinfo.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/commonplayoffseries.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/commonplayoffseries.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/commonteamroster.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/commonteamroster.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/commonteamyears.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/commonteamyears.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/cumestatsplayer.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/cumestatsplayer.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/cumestatsplayergames.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/cumestatsplayergames.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/cumestatsteam.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/cumestatsteam.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/cumestatsteamgames.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/cumestatsteamgames.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/defensehub.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/defensehub.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/draftboard.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/draftboard.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/draftcombinedrillresults.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/draftcombinedrillresults.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/draftcombinenonstationaryshooting.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/draftcombinenonstationaryshooting.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/draftcombineplayeranthro.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/draftcombineplayeranthro.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/draftcombinespotshooting.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/draftcombinespotshooting.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/draftcombinestats.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/draftcombinestats.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/drafthistory.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/drafthistory.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/fantasywidget.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/fantasywidget.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/franchisehistory.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/franchisehistory.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/franchiseleaders.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/franchiseleaders.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/franchiseplayers.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/franchiseplayers.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/gamerotation.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/gamerotation.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/glalumboxscoresimilarityscore.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/glalumboxscoresimilarityscore.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/homepageleaders.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/homepageleaders.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/homepagev2.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/homepagev2.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/hustlestatsboxscore.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/hustlestatsboxscore.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/infographicfanduelplayer.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/infographicfanduelplayer.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/leaderstiles.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/leaderstiles.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/leaguedashlineups.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/leaguedashlineups.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/leaguedashoppptshot.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/leaguedashoppptshot.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/leaguedashplayerbiostats.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/leaguedashplayerbiostats.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/leaguedashplayerclutch.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/leaguedashplayerclutch.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/leaguedashplayerptshot.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/leaguedashplayerptshot.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/leaguedashplayershotlocations.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/leaguedashplayershotlocations.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/leaguedashplayerstats.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/leaguedashplayerstats.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/leaguedashptdefend.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/leaguedashptdefend.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/leaguedashptstats.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/leaguedashptstats.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/leaguedashptteamdefend.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/leaguedashptteamdefend.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/leaguedashteamclutch.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/leaguedashteamclutch.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/leaguedashteamptshot.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/leaguedashteamptshot.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/leaguedashteamshotlocations.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/leaguedashteamshotlocations.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/leaguedashteamstats.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/leaguedashteamstats.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/leaguegamefinder.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/leaguegamefinder.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/leaguegamelog.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/leaguegamelog.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/leaguehustlestatsplayer.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/leaguehustlestatsplayer.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/leaguehustlestatsplayerleaders.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/leaguehustlestatsplayerleaders.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/leaguehustlestatsteam.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/leaguehustlestatsteam.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/leaguehustlestatsteamleaders.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/leaguehustlestatsteamleaders.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/leagueleaders.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/leagueleaders.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/leaguelineupviz.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/leaguelineupviz.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/leagueplayerondetails.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/leagueplayerondetails.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/leagueseasonmatchups.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/leagueseasonmatchups.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/leaguestandings.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/leaguestandings.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/leaguestandingsv3.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/leaguestandingsv3.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/matchupsrollup.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/matchupsrollup.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/playbyplay.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/playbyplay.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/playbyplayv2.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/playbyplayv2.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/playerawards.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/playerawards.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/playercareerbycollege.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/playercareerbycollege.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/playercareerbycollegerollup.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/playercareerbycollegerollup.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/playercareerstats.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/playercareerstats.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/playercompare.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/playercompare.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/playerdashboardbyclutch.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/playerdashboardbyclutch.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/playerdashboardbygamesplits.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/playerdashboardbygamesplits.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/playerdashboardbygeneralsplits.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/playerdashboardbygeneralsplits.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/playerdashboardbylastngames.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/playerdashboardbylastngames.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/playerdashboardbyopponent.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/playerdashboardbyopponent.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/playerdashboardbyshootingsplits.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/playerdashboardbyshootingsplits.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/playerdashboardbyteamperformance.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/playerdashboardbyteamperformance.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/playerdashboardbyyearoveryear.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/playerdashboardbyyearoveryear.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/playerdashptpass.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/playerdashptpass.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/playerdashptreb.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/playerdashptreb.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/playerdashptshotdefend.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/playerdashptshotdefend.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/playerdashptshots.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/playerdashptshots.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/playerestimatedmetrics.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/playerestimatedmetrics.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/playerfantasyprofile.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/playerfantasyprofile.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/playerfantasyprofilebargraph.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/playerfantasyprofilebargraph.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/playergamelog.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/playergamelog.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/playergamelogs.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/playergamelogs.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/playergamestreakfinder.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/playergamestreakfinder.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/playerindex.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/playerindex.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,20 +50,21 @@
             'TeamID': team_id_nullable,
             'Weight': weight_nullable
         }
         if get_request:
             self.get_request()
 
     def get_request(self):
-        self.nba_responce = NBAStatsHTTP().send_api_request(
+        self.nba_response = NBAStatsHTTP().send_api_request(
             endpoint=self.endpoint,
             parameters=self.parameters,
             proxy=self.proxy,
             headers=self.headers,
             timeout=self.timeout
         )
-        self.load_responce()
+        self.load_response()
 
-    def load_responce(self):
-        data_sets = self.nba_responce.get_data_sets()
-        self.data_sets = [Endpoint.DataSet(data=data_sets) for data_set_name, data_set in data_sets.items()]
+    def load_response(self):
+        data_sets = self.nba_response.get_data_sets()
+        self.data_sets = [Endpoint.DataSet(data=data_set) for data_set_name, data_set in data_sets.items()]
         self.player_index = Endpoint.DataSet(data=data_sets["PlayerIndex"])
+
```

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/playernextngames.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/playernextngames.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/playerprofilev2.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/playerprofilev2.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/playervsplayer.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/playervsplayer.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/playoffpicture.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/playoffpicture.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/scoreboard.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/scoreboard.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/scoreboardv2.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/scoreboardv2.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/shotchartdetail.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/shotchartdetail.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/shotchartleaguewide.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/shotchartleaguewide.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/shotchartlineupdetail.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/shotchartlineupdetail.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/synergyplaytypes.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/synergyplaytypes.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/teamandplayersvsplayers.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/teamandplayersvsplayers.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/teamdashboardbyclutch.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/teamdashboardbyclutch.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/teamdashboardbygamesplits.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/teamdashboardbygamesplits.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/teamdashboardbygeneralsplits.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/teamdashboardbygeneralsplits.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/teamdashboardbylastngames.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/teamdashboardbylastngames.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/teamdashboardbyopponent.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/teamdashboardbyopponent.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/teamdashboardbyshootingsplits.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/teamdashboardbyshootingsplits.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/teamdashboardbyteamperformance.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/teamdashboardbyteamperformance.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/teamdashboardbyyearoveryear.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/teamdashboardbyyearoveryear.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/teamdashlineups.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/teamdashlineups.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/teamdashptpass.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/teamdashptpass.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/teamdashptreb.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/teamdashptreb.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/teamdashptshots.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/teamdashptshots.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/teamdetails.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/teamdetails.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/teamestimatedmetrics.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/teamestimatedmetrics.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/teamgamelog.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/teamgamelog.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/teamgamelogs.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/teamgamelogs.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/teamgamestreakfinder.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/teamgamestreakfinder.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/teamhistoricalleaders.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/teamhistoricalleaders.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/teaminfocommon.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/teaminfocommon.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/teamplayerdashboard.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/teamplayerdashboard.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/teamplayeronoffdetails.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/teamplayeronoffdetails.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/teamplayeronoffsummary.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/teamplayeronoffsummary.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/teamvsplayer.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/teamvsplayer.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/teamyearbyyearstats.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/teamyearbyyearstats.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/videodetails.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/videodetails.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/videodetailsasset.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/videodetailsasset.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/videoevents.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/videoevents.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/videoeventsasset.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/videoeventsasset.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/videostatus.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/videostatus.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/endpoints/winprobabilitypbp.py` & `nba_api-1.2.1/src/nba_api/stats/endpoints/winprobabilitypbp.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/library/data.py` & `nba_api-1.2.1/src/nba_api/stats/library/data.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/library/http.py` & `nba_api-1.2.1/src/nba_api/stats/library/http.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/library/parameters.py` & `nba_api-1.2.1/src/nba_api/stats/library/parameters.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/library/playbyplayregex.py` & `nba_api-1.2.1/src/nba_api/stats/library/playbyplayregex.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/static/players.py` & `nba_api-1.2.1/src/nba_api/stats/static/players.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/src/nba_api/stats/static/teams.py` & `nba_api-1.2.1/src/nba_api/stats/static/teams.py`

 * *Files identical despite different names*

### Comparing `nba_api-1.2/PKG-INFO` & `nba_api-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nba-api
-Version: 1.2
+Version: 1.2.1
 Summary: An API Client package to access the APIs for NBA.com
 Home-page: https://github.com/swar/nba_api
 License: MIT
 Keywords: api,basketball,data,nba,sports,stats
 Author: Swar Patel
 Author-email: swar.m.patel@gmail.com
 Maintainer: Swar Patel
@@ -98,15 +98,15 @@
 - Static Data Sets
   - [players.py](https://github.com/swar/nba_api/tree/master/docs/nba_api/stats/static/players.md)
   - [teams.py](https://github.com/swar/nba_api/tree/master/docs/nba_api/stats/static/teams.md)
 
 # Join the Community
 ## Slack
 
-Join [Slack](https://join.slack.com/t/nbaapi/shared_invite/zt-1ipsuai9j-GjZjuP9S2~Uczuny1t74zA) to get help, help others, provide feedback, see amazing projects, participates in discussions, and collaborate with others from around the world.
+Join [Slack](https://join.slack.com/t/nbaapi/shared_invite/zt-cayfrnfo-s9rySAmBXxBloL09S6N0KA) to get help, help others, provide feedback, see amazing projects, participates in discussions, and collaborate with others from around the world.
 
 ## Stack Overflow
 
 Not a Slack fan? No problem. Head over to [StackOverflow](https://stackoverflow.com/questions/tagged/nba-api). Be sure to tag your post with `nba-api`.
 
 # Contributing
```

