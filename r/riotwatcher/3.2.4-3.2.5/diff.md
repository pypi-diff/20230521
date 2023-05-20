# Comparing `tmp/riotwatcher-3.2.4.tar.gz` & `tmp/riotwatcher-3.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riotwatcher-3.2.4.tar", last modified: Sun Oct 30 18:39:02 2022, max compression
+gzip compressed data, was "riotwatcher-3.2.5.tar", last modified: Sat May 20 22:41:01 2023, max compression
```

## Comparing `riotwatcher-3.2.4.tar` & `riotwatcher-3.2.5.tar`

### file list

```diff
@@ -1,115 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 18:39:02.841599 riotwatcher-3.2.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1095 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    16271 2022-10-30 18:39:02.837599 riotwatcher-3.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    15713 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-30 18:39:02.841599 riotwatcher-3.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1236 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 18:39:02.817599 riotwatcher-3.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 18:39:02.821599 riotwatcher-3.2.4/src/riotwatcher/
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/Deserializer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 18:39:02.825599 riotwatcher-3.2.4/src/riotwatcher/Handlers/
--rw-r--r--   0 runner    (1001) docker     (121)     1372 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/Handlers/DeprecationHandler.py
--rw-r--r--   0 runner    (1001) docker     (121)      713 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/Handlers/DeserializerAdapter.py
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/Handlers/DictionaryDeserializer.py
--rw-r--r--   0 runner    (1001) docker     (121)      373 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/Handlers/IllegalArgumentError.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 18:39:02.825599 riotwatcher-3.2.4/src/riotwatcher/Handlers/RateLimit/
--rw-r--r--   0 runner    (1001) docker     (121)      327 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/Handlers/RateLimit/ApplicationRateLimiter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1851 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/Handlers/RateLimit/BasicRateLimiter.py
--rw-r--r--   0 runner    (1001) docker     (121)     3852 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/Handlers/RateLimit/HeaderBasedLimiter.py
--rw-r--r--   0 runner    (1001) docker     (121)      447 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/Handlers/RateLimit/InternalLimiter.py
--rw-r--r--   0 runner    (1001) docker     (121)     4032 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/Handlers/RateLimit/Limits.py
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/Handlers/RateLimit/MethodRateLimiter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1527 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/Handlers/RateLimit/OopsRateLimiter.py
--rw-r--r--   0 runner    (1001) docker     (121)      544 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/Handlers/RateLimit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2187 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/Handlers/RateLimiterAdapter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1841 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/Handlers/RequestHandler.py
--rw-r--r--   0 runner    (1001) docker     (121)     1221 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/Handlers/SanitationHandler.py
--rw-r--r--   0 runner    (1001) docker     (121)      495 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/Handlers/ThrowOnErrorHandler.py
--rw-r--r--   0 runner    (1001) docker     (121)     1562 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/Handlers/TypeCorrectorHandler.py
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/Handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7552 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/LolWatcher.py
--rw-r--r--   0 runner    (1001) docker     (121)     2403 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/LorWatcher.py
--rw-r--r--   0 runner    (1001) docker     (121)      464 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/RateLimiter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2663 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/TftWatcher.py
--rw-r--r--   0 runner    (1001) docker     (121)     2357 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/ValWatcher.py
--rw-r--r--   0 runner    (1001) docker     (121)      609 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 18:39:02.829599 riotwatcher-3.2.4/src/riotwatcher/_apis/
--rw-r--r--   0 runner    (1001) docker     (121)     2687 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/BaseApi.py
--rw-r--r--   0 runner    (1001) docker     (121)      744 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/Endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     1437 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/NamedEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/UrlConfig.py
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1144 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 18:39:02.829599 riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/
--rw-r--r--   0 runner    (1001) docker     (121)     3680 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/ChallengesApiV1.py
--rw-r--r--   0 runner    (1001) docker     (121)      909 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/ChampionApiV3.py
--rw-r--r--   0 runner    (1001) docker     (121)     3029 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/ChampionMasteryApiV4.py
--rw-r--r--   0 runner    (1001) docker     (121)     3285 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/ClashApiV1.py
--rw-r--r--   0 runner    (1001) docker     (121)     2044 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/DataDragonApi.py
--rw-r--r--   0 runner    (1001) docker     (121)     3875 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/LeagueApiV4.py
--rw-r--r--   0 runner    (1001) docker     (121)     1024 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/LolStatusApiV3.py
--rw-r--r--   0 runner    (1001) docker     (121)     1039 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/LolStatusApiV4.py
--rw-r--r--   0 runner    (1001) docker     (121)     3727 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/MatchApiV5.py
--rw-r--r--   0 runner    (1001) docker     (121)     1495 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/SpectatorApiV4.py
--rw-r--r--   0 runner    (1001) docker     (121)     2623 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/SummonerApiV4.py
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 18:39:02.833599 riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/urls/
--rw-r--r--   0 runner    (1001) docker     (121)      721 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/urls/ChallengesApiV1Urls.py
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/urls/ChampionApiUrls.py
--rw-r--r--   0 runner    (1001) docker     (121)      636 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/urls/ChampionMasteryApiUrls.py
--rw-r--r--   0 runner    (1001) docker     (121)      551 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/urls/ClashApiUrls.py
--rw-r--r--   0 runner    (1001) docker     (121)     1174 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/urls/DataDragonUrls.py
--rw-r--r--   0 runner    (1001) docker     (121)      679 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/urls/LeagueApiUrls.py
--rw-r--r--   0 runner    (1001) docker     (121)      311 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/urls/LeagueEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/urls/LolStatusApiUrls.py
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/urls/LolStatusApiV4Urls.py
--rw-r--r--   0 runner    (1001) docker     (121)      503 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/urls/MatchApiV5Urls.py
--rw-r--r--   0 runner    (1001) docker     (121)      395 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/urls/SpectatorApiUrls.py
--rw-r--r--   0 runner    (1001) docker     (121)      499 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/urls/SummonerApiUrls.py
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/urls/ThirdPartyCodeApiUrls.py
--rw-r--r--   0 runner    (1001) docker     (121)      586 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/urls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 18:39:02.833599 riotwatcher-3.2.4/src/riotwatcher/_apis/legends_of_runeterra/
--rw-r--r--   0 runner    (1001) docker     (121)     1097 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/legends_of_runeterra/MatchApi.py
--rw-r--r--   0 runner    (1001) docker     (121)      835 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/legends_of_runeterra/RankedApi.py
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/legends_of_runeterra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 18:39:02.833599 riotwatcher-3.2.4/src/riotwatcher/_apis/legends_of_runeterra/urls/
--rw-r--r--   0 runner    (1001) docker     (121)      307 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/legends_of_runeterra/urls/LorEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)      304 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/legends_of_runeterra/urls/MatchApiUrls.py
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/legends_of_runeterra/urls/RankedApiUrls.py
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/legends_of_runeterra/urls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 18:39:02.837599 riotwatcher-3.2.4/src/riotwatcher/_apis/riot/
--rw-r--r--   0 runner    (1001) docker     (121)     1551 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/riot/AccountApi.py
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/riot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 18:39:02.837599 riotwatcher-3.2.4/src/riotwatcher/_apis/riot/urls/
--rw-r--r--   0 runner    (1001) docker     (121)      428 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/riot/urls/AccountApiUrls.py
--rw-r--r--   0 runner    (1001) docker     (121)      310 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/riot/urls/RiotEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/riot/urls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 18:39:02.837599 riotwatcher-3.2.4/src/riotwatcher/_apis/team_fight_tactics/
--rw-r--r--   0 runner    (1001) docker     (121)     2719 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/team_fight_tactics/LeagueApi.py
--rw-r--r--   0 runner    (1001) docker     (121)     1761 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/team_fight_tactics/MatchApi.py
--rw-r--r--   0 runner    (1001) docker     (121)     1898 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/team_fight_tactics/SummonerApi.py
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/team_fight_tactics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 18:39:02.837599 riotwatcher-3.2.4/src/riotwatcher/_apis/team_fight_tactics/urls/
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/team_fight_tactics/urls/LeagueApiUrls.py
--rw-r--r--   0 runner    (1001) docker     (121)      338 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/team_fight_tactics/urls/MatchApiUrls.py
--rw-r--r--   0 runner    (1001) docker     (121)      473 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/team_fight_tactics/urls/SummonerApiUrls.py
--rw-r--r--   0 runner    (1001) docker     (121)      307 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/team_fight_tactics/urls/TftEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/team_fight_tactics/urls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 18:39:02.837599 riotwatcher-3.2.4/src/riotwatcher/_apis/valorant/
--rw-r--r--   0 runner    (1001) docker     (121)      870 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/valorant/ContentApi.py
--rw-r--r--   0 runner    (1001) docker     (121)     1847 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/valorant/MatchApi.py
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/valorant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 18:39:02.837599 riotwatcher-3.2.4/src/riotwatcher/_apis/valorant/urls/
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/valorant/urls/ContentApiUrls.py
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/valorant/urls/MatchApiUrls.py
--rw-r--r--   0 runner    (1001) docker     (121)      307 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/valorant/urls/ValEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/_apis/valorant/urls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      271 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2121 2022-10-30 18:38:35.000000 riotwatcher-3.2.4/src/riotwatcher/riotwatcher.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 18:39:02.825599 riotwatcher-3.2.4/src/riotwatcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    16271 2022-10-30 18:39:02.000000 riotwatcher-3.2.4/src/riotwatcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4713 2022-10-30 18:39:02.000000 riotwatcher-3.2.4/src/riotwatcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-30 18:39:02.000000 riotwatcher-3.2.4/src/riotwatcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-10-30 18:39:02.000000 riotwatcher-3.2.4/src/riotwatcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-10-30 18:39:02.000000 riotwatcher-3.2.4/src/riotwatcher.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 22:41:01.346981 riotwatcher-3.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16270 2023-05-20 22:41:01.346981 riotwatcher-3.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15712 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 22:41:01.346981 riotwatcher-3.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 22:41:01.326981 riotwatcher-3.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 22:41:01.330981 riotwatcher-3.2.5/src/riotwatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/Deserializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 22:41:01.334981 riotwatcher-3.2.5/src/riotwatcher/Handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/Handlers/DeprecationHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/Handlers/DeserializerAdapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/Handlers/DictionaryDeserializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/Handlers/IllegalArgumentError.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 22:41:01.334981 riotwatcher-3.2.5/src/riotwatcher/Handlers/RateLimit/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/Handlers/RateLimit/ApplicationRateLimiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/Handlers/RateLimit/BasicRateLimiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/Handlers/RateLimit/HeaderBasedLimiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/Handlers/RateLimit/InternalLimiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/Handlers/RateLimit/Limits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/Handlers/RateLimit/MethodRateLimiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/Handlers/RateLimit/OopsRateLimiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/Handlers/RateLimit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/Handlers/RateLimiterAdapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/Handlers/RequestHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/Handlers/SanitationHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/Handlers/ThrowOnErrorHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/Handlers/TypeCorrectorHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/Handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/LolWatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/LorWatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/RateLimiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/TftWatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/ValWatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 22:41:01.338981 riotwatcher-3.2.5/src/riotwatcher/_apis/
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/BaseApi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/Endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/NamedEndpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/UrlConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 22:41:01.338981 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/ChallengesApiV1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/ChampionApiV3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/ChampionMasteryApiV4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/ClashApiV1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/DataDragonApi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/LeagueApiV4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/LolStatusApiV3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/LolStatusApiV4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/MatchApiV5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/SpectatorApiV4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/SummonerApiV4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 22:41:01.342981 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/ChallengesApiV1Urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/ChampionApiUrls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/ChampionMasteryApiUrls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/ClashApiUrls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/DataDragonUrls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/LeagueApiUrls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/LeagueEndpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/LolStatusApiUrls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/LolStatusApiV4Urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/MatchApiV5Urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/SpectatorApiUrls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/SummonerApiUrls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/ThirdPartyCodeApiUrls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 22:41:01.342981 riotwatcher-3.2.5/src/riotwatcher/_apis/legends_of_runeterra/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/legends_of_runeterra/MatchApi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/legends_of_runeterra/RankedApi.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/legends_of_runeterra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 22:41:01.342981 riotwatcher-3.2.5/src/riotwatcher/_apis/legends_of_runeterra/urls/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/legends_of_runeterra/urls/LorEndpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/legends_of_runeterra/urls/MatchApiUrls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/legends_of_runeterra/urls/RankedApiUrls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/legends_of_runeterra/urls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 22:41:01.342981 riotwatcher-3.2.5/src/riotwatcher/_apis/riot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/riot/AccountApi.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/riot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 22:41:01.342981 riotwatcher-3.2.5/src/riotwatcher/_apis/riot/urls/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/riot/urls/AccountApiUrls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/riot/urls/RiotEndpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/riot/urls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 22:41:01.346981 riotwatcher-3.2.5/src/riotwatcher/_apis/team_fight_tactics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/team_fight_tactics/LeagueApi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/team_fight_tactics/MatchApi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/team_fight_tactics/SummonerApi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/team_fight_tactics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 22:41:01.346981 riotwatcher-3.2.5/src/riotwatcher/_apis/team_fight_tactics/urls/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/team_fight_tactics/urls/LeagueApiUrls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/team_fight_tactics/urls/MatchApiUrls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/team_fight_tactics/urls/SummonerApiUrls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/team_fight_tactics/urls/TftEndpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/team_fight_tactics/urls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 22:41:01.346981 riotwatcher-3.2.5/src/riotwatcher/_apis/valorant/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/valorant/ContentApi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/valorant/MatchApi.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/valorant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 22:41:01.346981 riotwatcher-3.2.5/src/riotwatcher/_apis/valorant/urls/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/valorant/urls/ContentApiUrls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/valorant/urls/MatchApiUrls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/valorant/urls/ValEndpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/valorant/urls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/riotwatcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 22:41:01.330981 riotwatcher-3.2.5/src/riotwatcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16270 2023-05-20 22:41:01.000000 riotwatcher-3.2.5/src/riotwatcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-05-20 22:41:01.000000 riotwatcher-3.2.5/src/riotwatcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 22:41:01.000000 riotwatcher-3.2.5/src/riotwatcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-20 22:41:01.000000 riotwatcher-3.2.5/src/riotwatcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-20 22:41:01.000000 riotwatcher-3.2.5/src/riotwatcher.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 22:41:01.346981 riotwatcher-3.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/tests/test_LolWatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/tests/test_LorWatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/tests/test_RiotWatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/tests/test_TftWatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/tests/test_ValWatcher.py
```

### Comparing `riotwatcher-3.2.4/LICENSE` & `riotwatcher-3.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/PKG-INFO` & `riotwatcher-3.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: riotwatcher
-Version: 3.2.4
+Version: 3.2.5
 Summary: RiotWatcher is a thin wrapper on top of the Riot Games API for League of Legends.
 Home-page: https://github.com/pseudonym117/Riot-Watcher
 Author: AG Stephan
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing
@@ -18,15 +18,15 @@
 
 |pypi| |docs| |coverage| |black|
 
 Check for full (read: slightly better) documentation `here <http://riot-watcher.readthedocs.io/en/latest/>`__!
 
 RiotWatcher is a thin wrapper on top of the `Riot Games API for League
 of Legends <https://developer.riotgames.com/>`__. All public methods as
-of 10/29/2022 are supported in full.
+of 5/20/2023 are supported in full.
 
 RiotWatcher by default supports a naive rate limiter. This rate limiter will
 try to stop you from making too many requests, and in a single threaded test
 environment does this rather well. In a multithreaded environment, you may
 still get some 429 errors. 429 errors are currently NOT retried for you.
```

### Comparing `riotwatcher-3.2.4/README.rst` & `riotwatcher-3.2.5/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 |pypi| |docs| |coverage| |black|
 
 Check for full (read: slightly better) documentation `here <http://riot-watcher.readthedocs.io/en/latest/>`__!
 
 RiotWatcher is a thin wrapper on top of the `Riot Games API for League
 of Legends <https://developer.riotgames.com/>`__. All public methods as
-of 10/29/2022 are supported in full.
+of 5/20/2023 are supported in full.
 
 RiotWatcher by default supports a naive rate limiter. This rate limiter will
 try to stop you from making too many requests, and in a single threaded test
 environment does this rather well. In a multithreaded environment, you may
 still get some 429 errors. 429 errors are currently NOT retried for you.
```

### Comparing `riotwatcher-3.2.4/setup.py` & `riotwatcher-3.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/Handlers/DeprecationHandler.py` & `riotwatcher-3.2.5/src/riotwatcher/Handlers/DeprecationHandler.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/Handlers/DeserializerAdapter.py` & `riotwatcher-3.2.5/src/riotwatcher/Handlers/DeserializerAdapter.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/Handlers/RateLimit/BasicRateLimiter.py` & `riotwatcher-3.2.5/src/riotwatcher/Handlers/RateLimit/BasicRateLimiter.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/Handlers/RateLimit/HeaderBasedLimiter.py` & `riotwatcher-3.2.5/src/riotwatcher/Handlers/RateLimit/HeaderBasedLimiter.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/Handlers/RateLimit/Limits.py` & `riotwatcher-3.2.5/src/riotwatcher/Handlers/RateLimit/Limits.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/Handlers/RateLimit/OopsRateLimiter.py` & `riotwatcher-3.2.5/src/riotwatcher/Handlers/RateLimit/OopsRateLimiter.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/Handlers/RateLimit/__init__.py` & `riotwatcher-3.2.5/src/riotwatcher/Handlers/RateLimit/__init__.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/Handlers/RateLimiterAdapter.py` & `riotwatcher-3.2.5/src/riotwatcher/Handlers/RateLimiterAdapter.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/Handlers/RequestHandler.py` & `riotwatcher-3.2.5/src/riotwatcher/Handlers/RequestHandler.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/Handlers/SanitationHandler.py` & `riotwatcher-3.2.5/src/riotwatcher/Handlers/SanitationHandler.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/Handlers/TypeCorrectorHandler.py` & `riotwatcher-3.2.5/src/riotwatcher/Handlers/TypeCorrectorHandler.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/LolWatcher.py` & `riotwatcher-3.2.5/src/riotwatcher/LolWatcher.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/LorWatcher.py` & `riotwatcher-3.2.5/src/riotwatcher/LorWatcher.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/TftWatcher.py` & `riotwatcher-3.2.5/src/riotwatcher/TftWatcher.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/ValWatcher.py` & `riotwatcher-3.2.5/src/riotwatcher/ValWatcher.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/__init__.py` & `riotwatcher-3.2.5/src/riotwatcher/__init__.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/_apis/BaseApi.py` & `riotwatcher-3.2.5/src/riotwatcher/_apis/BaseApi.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/_apis/Endpoint.py` & `riotwatcher-3.2.5/src/riotwatcher/_apis/Endpoint.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/_apis/NamedEndpoint.py` & `riotwatcher-3.2.5/src/riotwatcher/_apis/NamedEndpoint.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/_apis/helpers.py` & `riotwatcher-3.2.5/src/riotwatcher/_apis/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,19 @@
     def _remap_region_to_platform(api_call):
         remap = {
             "br1": "americas",
             "la1": "americas",
             "la2": "americas",
             "na1": "americas",
             "oc1": "sea",
+            "ph2": "sea",
+            "sg2": "sea",
+            "th2": "sea",
+            "tw2": "sea",
+            "vn2": "sea",
             "eun1": "europe",
             "euw1": "europe",
             "ru": "europe",
             "tr1": "europe",
             "jp1": "asia",
             "kr": "asia",
         }
```

### Comparing `riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/ChallengesApiV1.py` & `riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/ChallengesApiV1.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/ChampionApiV3.py` & `riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/ChampionApiV3.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/ChampionMasteryApiV4.py` & `riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/ChampionMasteryApiV4.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/ClashApiV1.py` & `riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/ClashApiV1.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/DataDragonApi.py` & `riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/DataDragonApi.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/LeagueApiV4.py` & `riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/LeagueApiV4.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/LolStatusApiV3.py` & `riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/LolStatusApiV3.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/LolStatusApiV4.py` & `riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/LolStatusApiV4.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/MatchApiV5.py` & `riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/MatchApiV5.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,22 +80,22 @@
             queue=queue,
             type=type,
             startTime=start_time,
             endTime=end_time,
         )
 
     @remap_region_to_platform(1)
-    def timeline_by_match(self, region: str, match_id: int):
+    def timeline_by_match(self, region: str, match_id: str):
         """
         Get match timeline by match ID.
 
         Not all matches have timeline data.
 
         :param string region: The region to execute this request on
-        :param long match_id: The match ID.
+        :param string match_id: The match ID.
 
         :returns: MatchTimelineDto
         """
         return self._request_endpoint(
             self.timeline_by_match.__name__,
             region,
             MatchApiV5Urls.timeline_by_match,
```

### Comparing `riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/SpectatorApiV4.py` & `riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/SpectatorApiV4.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/SummonerApiV4.py` & `riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/SummonerApiV4.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/urls/ChallengesApiV1Urls.py` & `riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/ChallengesApiV1Urls.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/urls/ChampionMasteryApiUrls.py` & `riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/ChampionMasteryApiUrls.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/urls/ClashApiUrls.py` & `riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/ClashApiUrls.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/urls/DataDragonUrls.py` & `riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/DataDragonUrls.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/urls/LeagueApiUrls.py` & `riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/LeagueApiUrls.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/_apis/league_of_legends/urls/__init__.py` & `riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/__init__.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/_apis/legends_of_runeterra/MatchApi.py` & `riotwatcher-3.2.5/src/riotwatcher/_apis/legends_of_runeterra/MatchApi.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/_apis/legends_of_runeterra/RankedApi.py` & `riotwatcher-3.2.5/src/riotwatcher/_apis/legends_of_runeterra/RankedApi.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/_apis/riot/AccountApi.py` & `riotwatcher-3.2.5/src/riotwatcher/_apis/riot/AccountApi.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/_apis/team_fight_tactics/LeagueApi.py` & `riotwatcher-3.2.5/src/riotwatcher/_apis/team_fight_tactics/LeagueApi.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/_apis/team_fight_tactics/MatchApi.py` & `riotwatcher-3.2.5/src/riotwatcher/_apis/team_fight_tactics/MatchApi.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from .. import BaseApi, NamedEndpoint
 from ..helpers import remap_region_to_platform
 from .urls import MatchApiUrls
 
+from typing import Optional
+
 
 class MatchApi(NamedEndpoint):
     """
     This class wraps the TFT-Match-v1 Api calls provided by the Riot API.
 
     See https://developer.riotgames.com/apis#tft-match-v1 for more detailed information
     """
@@ -15,33 +17,53 @@
         Initializes a new MatchApi which uses the provided base_api
 
         :param BaseApi base_api: the root API object to use for making all requests.
         """
         super().__init__(base_api, self.__class__.__name__)
 
     @remap_region_to_platform(1)
-    def by_puuid(self, region: str, puuid: str, count: int = 20, start: int = 0):
+    def by_puuid(
+        self,
+        region: str,
+        puuid: str,
+        count: int = 20,
+        start: int = 0,
+        start_time: Optional[int] = None,
+        end_time: Optional[int] = None,
+    ):
         """
         Get a list of match ids by PUUID.
 
         :param string region:   The region to execute this request on
         :param string puuid:    The puuid.
         :param int count:       Defaults to 20. Valid values: 0 to 100. Number of
                                 match ids to return.
         :param int start:       Defaults to 0. Start index.
+        :param int start_time:  Epoch timestamp in seconds.
+        :param int end_time:    Epoch timestamp in seconds.
 
         :returns: List[string]
         """
+        args = {
+            "count": count,
+            "start": start,
+        }
+
+        if start_time:
+            args["startTime"] = start_time
+
+        if end_time:
+            args["endTime"] = end_time
+
         return self._request_endpoint(
             self.by_puuid.__name__,
             region,
             MatchApiUrls.by_puuid,
             puuid=puuid,
-            start=start,
-            count=count,
+            **args,
         )
 
     @remap_region_to_platform(1)
     def by_id(self, region: str, match_id: str):
         """
         Get a match by match id.
```

### Comparing `riotwatcher-3.2.4/src/riotwatcher/_apis/team_fight_tactics/SummonerApi.py` & `riotwatcher-3.2.5/src/riotwatcher/_apis/team_fight_tactics/SummonerApi.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/_apis/team_fight_tactics/urls/LeagueApiUrls.py` & `riotwatcher-3.2.5/src/riotwatcher/_apis/team_fight_tactics/urls/LeagueApiUrls.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/_apis/valorant/ContentApi.py` & `riotwatcher-3.2.5/src/riotwatcher/_apis/valorant/ContentApi.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/_apis/valorant/MatchApi.py` & `riotwatcher-3.2.5/src/riotwatcher/_apis/valorant/MatchApi.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher/riotwatcher.py` & `riotwatcher-3.2.5/src/riotwatcher/riotwatcher.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.4/src/riotwatcher.egg-info/PKG-INFO` & `riotwatcher-3.2.5/src/riotwatcher.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: riotwatcher
-Version: 3.2.4
+Version: 3.2.5
 Summary: RiotWatcher is a thin wrapper on top of the Riot Games API for League of Legends.
 Home-page: https://github.com/pseudonym117/Riot-Watcher
 Author: AG Stephan
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing
@@ -18,15 +18,15 @@
 
 |pypi| |docs| |coverage| |black|
 
 Check for full (read: slightly better) documentation `here <http://riot-watcher.readthedocs.io/en/latest/>`__!
 
 RiotWatcher is a thin wrapper on top of the `Riot Games API for League
 of Legends <https://developer.riotgames.com/>`__. All public methods as
-of 10/29/2022 are supported in full.
+of 5/20/2023 are supported in full.
 
 RiotWatcher by default supports a naive rate limiter. This rate limiter will
 try to stop you from making too many requests, and in a single threaded test
 environment does this rather well. In a multithreaded environment, you may
 still get some 429 errors. 429 errors are currently NOT retried for you.
```

### Comparing `riotwatcher-3.2.4/src/riotwatcher.egg-info/SOURCES.txt` & `riotwatcher-3.2.5/src/riotwatcher.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -89,8 +89,13 @@
 src/riotwatcher/_apis/team_fight_tactics/urls/__init__.py
 src/riotwatcher/_apis/valorant/ContentApi.py
 src/riotwatcher/_apis/valorant/MatchApi.py
 src/riotwatcher/_apis/valorant/__init__.py
 src/riotwatcher/_apis/valorant/urls/ContentApiUrls.py
 src/riotwatcher/_apis/valorant/urls/MatchApiUrls.py
 src/riotwatcher/_apis/valorant/urls/ValEndpoint.py
-src/riotwatcher/_apis/valorant/urls/__init__.py
+src/riotwatcher/_apis/valorant/urls/__init__.py
+tests/test_LolWatcher.py
+tests/test_LorWatcher.py
+tests/test_RiotWatcher.py
+tests/test_TftWatcher.py
+tests/test_ValWatcher.py
```

