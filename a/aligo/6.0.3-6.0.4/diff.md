# Comparing `tmp/aligo-6.0.3.tar.gz` & `tmp/aligo-6.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aligo-6.0.3.tar", last modified: Mon Jun 12 04:07:17 2023, max compression
+gzip compressed data, was "aligo-6.0.4.tar", last modified: Tue Jun 13 06:51:44 2023, max compression
```

## Comparing `aligo-6.0.3.tar` & `aligo-6.0.4.tar`

### file list

```diff
@@ -1,211 +1,214 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:07:17.291532 aligo-6.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-12 04:07:10.000000 aligo-6.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-06-12 04:07:17.291532 aligo-6.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-06-12 04:07:10.000000 aligo-6.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-12 04:07:10.000000 aligo-6.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-12 04:07:10.000000 aligo-6.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 04:07:17.291532 aligo-6.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:07:17.263532 aligo-6.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:07:17.263532 aligo-6.0.3/src/aligo/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-12 04:07:16.000000 aligo-6.0.3/src/aligo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:07:17.267532 aligo-6.0.3/src/aligo/apis/
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/apis/Album.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/apis/Aligo.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/apis/Audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/apis/Compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/apis/Copy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/apis/Create.py
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/apis/CustomShare.py
--rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/apis/Download.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/apis/Drive.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/apis/Duplicate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/apis/File.py
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/apis/Move.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/apis/Other.py
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/apis/Recyclebin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/apis/Search.py
--rw-r--r--   0 runner    (1001) docker     (123)    23039 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/apis/Share.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/apis/Star.py
--rw-r--r--   0 runner    (1001) docker     (123)    17897 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/apis/SyncFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/apis/Update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/apis/Video.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:07:17.271532 aligo-6.0.3/src/aligo/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/core/Album.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/core/Audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    19145 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/core/Auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/core/BaseAligo.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/core/Compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/core/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/core/Copy.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/core/Core.py
--rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/core/Create.py
--rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/core/Download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/core/Drive.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/core/Duplicate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/core/EMail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/core/File.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/core/LoginServer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/core/Move.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/core/Other.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/core/Recyclebin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/core/Search.py
--rw-r--r--   0 runner    (1001) docker     (123)     8958 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/core/Share.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/core/Star.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/core/Template.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/core/Update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/core/User.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/core/Video.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:07:17.271532 aligo-6.0.3/src/aligo/error/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/error/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:07:17.279532 aligo-6.0.3/src/aligo/request/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/AimSearchRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/AlbumListFilesRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/AlbumListRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/ArchiveStatusRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/ArchiveUncompressRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/BatchCancelShareRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/BatchCopyFilesRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/BatchDownloadUrlRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/BatchGetFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/BatchMoveFilesRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/BatchMoveToTrashRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/BatchRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/BatchRestoreRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/BatchShareFileSaveToDriveRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/BatchStarFilesRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/BatchSubRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/CancelShareLinkRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/CompleteFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/CopyFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/CreateFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/CreateFolderRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/CreateShareLinkRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/GetAudioPlayInfoRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/GetDefaultDriveRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/GetDownloadUrlRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/GetDriveRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/GetFileListRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/GetFilePathRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/GetFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/GetRecycleBinListRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/GetShareFileListRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/GetShareFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/GetShareInfoRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/GetShareLinkDownloadUrlRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/GetShareLinkListRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/GetShareTokenRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/GetStarredListRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/GetUploadUrlRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/GetVideoPlayInfoRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/GetVideoPreviewPlayInfoRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/ListToCleanRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/MoveFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/MoveFileToTrashRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/RenameFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/RestoreFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/SearchFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/SearchShareFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/ShareFileSaveToDriveRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/StarredFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/TemplateRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/UpdateFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/UpdateShareLinkRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/request/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:07:17.283532 aligo-6.0.3/src/aligo/response/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/AimSearchResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/AlbumInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/AlbumListResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/ArchiveStatusResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/ArchiveUncompressResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/BatchDownloadUrlResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/BatchShareFileSaveToDriveResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/BatchSubResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/CancelShareLinkResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/CopyFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/CreateFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/CreateShareLinkResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/DuplicateListResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/GetAudioPlayInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/GetDownloadUrlResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/GetFileListResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/GetFilePathResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/GetOfficePreviewUrlResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/GetPersonalInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/GetRecycleBinListResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/GetShareFileListResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/GetShareInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/GetShareLinkDownloadUrlResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/GetShareLinkListResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/GetShareTokenResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/GetStarredListResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/GetUploadUrlResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/GetVideoPlayInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/GetVideoPreviewPlayInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/ListMyDrivesResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/ListResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/ListToCleanResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/MoveFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/MoveFileToTrashResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/RestoreFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/RewardSpaceResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/SearchFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/SearchShareFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/ShareFileSaveToDriveResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/ShareItemInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/ShareLinkExtractCodeResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/TemplateResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/UpdateShareLinkResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/UsersVipInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/response/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:07:17.287532 aligo-6.0.3/src/aligo/types/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/AudioMeta.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/AudioMusicMeta.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/AudioTranscodeTemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/BaseAlbum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/BaseDrive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/BaseFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/BaseShareFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/BaseUser.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/CroppingBoundary.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/CroppingSuggestionItem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/DataClass.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/DriveCapacityDetail.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/EMailConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/Enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/FaceThumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/FieldsInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/FolderSizeInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/ImageMedia.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/ImageQuality.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/ImageTag.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/ListAlbumItem.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/LoginDevice.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/LoginTimout.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/MediaTransCodeTemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/Null.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/PersonalRightsInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/PersonalSpaceInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/Privilege.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/RateLimit.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/ShareLinkBaseFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/ShareLinkSchema.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/SystemTag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/Token.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/UploadPartInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/UserConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/VideoMedia.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/VideoMediaAudioStream.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/VideoMediaVideoStream.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/VideoPreview.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/VideoPreviewPlayInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/VideoPreviewSprite.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/VideoTranscodeTemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-12 04:07:10.000000 aligo-6.0.3/src/aligo/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:07:17.263532 aligo-6.0.3/src/aligo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-06-12 04:07:17.000000 aligo-6.0.3/src/aligo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-06-12 04:07:17.000000 aligo-6.0.3/src/aligo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 04:07:17.000000 aligo-6.0.3/src/aligo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-12 04:07:17.000000 aligo-6.0.3/src/aligo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 04:07:17.000000 aligo-6.0.3/src/aligo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:51:44.938837 aligo-6.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-13 06:51:38.000000 aligo-6.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-06-13 06:51:44.938837 aligo-6.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-06-13 06:51:38.000000 aligo-6.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-13 06:51:38.000000 aligo-6.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-13 06:51:38.000000 aligo-6.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 06:51:44.938837 aligo-6.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:51:44.914837 aligo-6.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:51:44.914837 aligo-6.0.4/src/aligo/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-13 06:51:44.000000 aligo-6.0.4/src/aligo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:51:44.918837 aligo-6.0.4/src/aligo/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/apis/Album.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/apis/Aligo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/apis/Audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/apis/Compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/apis/Copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/apis/Create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/apis/CustomShare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/apis/Download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/apis/Drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/apis/Duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/apis/File.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/apis/Move.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/apis/Other.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/apis/Recyclebin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/apis/Search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23234 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/apis/Share.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/apis/Star.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17897 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/apis/SyncFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/apis/Update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/apis/Video.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:51:44.922837 aligo-6.0.4/src/aligo/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/core/Album.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/core/Audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19145 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/core/Auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/core/BaseAligo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/core/Compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/core/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/core/Copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/core/Core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/core/Create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/core/Download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/core/Drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/core/Duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/core/EMail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/core/File.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/core/LoginServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/core/Move.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/core/Other.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/core/Recyclebin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/core/Search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/core/Share.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/core/Star.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/core/Template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/core/Update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/core/User.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/core/Video.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:51:44.922837 aligo-6.0.4/src/aligo/error/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/error/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:51:44.926837 aligo-6.0.4/src/aligo/request/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/AimSearchRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/AlbumListFilesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/AlbumListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/ArchiveStatusRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/ArchiveUncompressRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/BatchCancelShareRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/BatchCopyFilesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/BatchDownloadUrlRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/BatchGetFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/BatchMoveFilesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/BatchMoveToTrashRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/BatchRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/BatchRestoreRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/BatchShareFileSaveToDriveRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/BatchStarFilesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/BatchSubRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/CancelShareLinkRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/CompleteFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/CopyFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/CreateFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/CreateFolderRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/CreateShareLinkRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/GetAudioPlayInfoRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/GetDefaultDriveRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/GetDownloadUrlRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/GetDriveRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/GetFileListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/GetFilePathRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/GetFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/GetRecycleBinListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/GetShareFileListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/GetShareFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/GetShareInfoRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/GetShareLinkDownloadUrlRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/GetShareLinkListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/GetShareTokenRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/GetStarredListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/GetUploadUrlRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/GetVideoPlayInfoRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/GetVideoPreviewPlayInfoRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/ListToCleanRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/MoveFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/MoveFileToTrashRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/PrivateShareRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/RenameFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/RestoreFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/SearchFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/SearchShareFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/ShareFileSaveToDriveRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/StarredFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/TemplateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/UpdateFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/UpdateShareLinkRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/request/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:51:44.934837 aligo-6.0.4/src/aligo/response/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/AimSearchResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/AlbumInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/AlbumListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/ArchiveStatusResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/ArchiveUncompressResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/BatchDownloadUrlResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/BatchShareFileSaveToDriveResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/BatchSubResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/CancelShareLinkResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/CopyFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/CreateFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/CreateShareLinkResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/DuplicateListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/GetAudioPlayInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/GetDownloadUrlResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/GetFileListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/GetFilePathResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/GetOfficePreviewUrlResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/GetPersonalInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/GetRecycleBinListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/GetShareFileListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/GetShareInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/GetShareLinkDownloadUrlResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/GetShareLinkListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/GetShareTokenResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/GetStarredListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/GetUploadUrlResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/GetVideoPlayInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/GetVideoPreviewPlayInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/ListMyDrivesResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/ListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/ListToCleanResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/MoveFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/MoveFileToTrashResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/PrivateShareResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/RestoreFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/RewardSpaceResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/SearchFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/SearchShareFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/ShareFileSaveToDriveResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/ShareItemInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/ShareLinkExtractCodeResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/TemplateResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/UpdateShareLinkResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/UsersVipInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/response/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:51:44.938837 aligo-6.0.4/src/aligo/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/AudioMeta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/AudioMusicMeta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/AudioTranscodeTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/BaseAlbum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/BaseDrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/BaseFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/BaseShareFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/BaseUser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/CroppingBoundary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/CroppingSuggestionItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/DataClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/DriveCapacityDetail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/DriveFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/EMailConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/Enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/FaceThumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/FieldsInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/FolderSizeInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/ImageMedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/ImageQuality.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/ImageTag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/ListAlbumItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/LoginDevice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/LoginTimout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/MediaTransCodeTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/Null.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/PersonalRightsInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/PersonalSpaceInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/Privilege.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/RateLimit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/ShareLinkBaseFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/ShareLinkSchema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/SystemTag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/Token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/UploadPartInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/UserConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/VideoMedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/VideoMediaAudioStream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/VideoMediaVideoStream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/VideoPreview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/VideoPreviewPlayInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/VideoPreviewSprite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/VideoTranscodeTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-13 06:51:38.000000 aligo-6.0.4/src/aligo/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:51:44.914837 aligo-6.0.4/src/aligo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-06-13 06:51:44.000000 aligo-6.0.4/src/aligo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-06-13 06:51:44.000000 aligo-6.0.4/src/aligo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 06:51:44.000000 aligo-6.0.4/src/aligo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-13 06:51:44.000000 aligo-6.0.4/src/aligo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 06:51:44.000000 aligo-6.0.4/src/aligo.egg-info/top_level.txt
```

### Comparing `aligo-6.0.3/LICENSE` & `aligo-6.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/PKG-INFO` & `aligo-6.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aligo
-Version: 6.0.3
+Version: 6.0.4
 Summary: aliyun drive sdk
 Author: foyoux
 Project-URL: Source, https://github.com/foyoux/aligo
 Project-URL: Homepage, https://github.com/foyoux/aligo
 Project-URL: Bug Tracker, https://github.com/foyoux/aligo/issues
 Keywords: aligo
 Classifier: Programming Language :: Python
```

### Comparing `aligo-6.0.3/README.md` & `aligo-6.0.4/README.md`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/pyproject.toml` & `aligo-6.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/apis/Album.py` & `aligo-6.0.4/src/aligo/apis/Album.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/apis/Aligo.py` & `aligo-6.0.4/src/aligo/apis/Aligo.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/apis/Audio.py` & `aligo-6.0.4/src/aligo/apis/Audio.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/apis/Compress.py` & `aligo-6.0.4/src/aligo/apis/Compress.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/apis/Copy.py` & `aligo-6.0.4/src/aligo/apis/Copy.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/apis/Create.py` & `aligo-6.0.4/src/aligo/apis/Create.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/apis/CustomShare.py` & `aligo-6.0.4/src/aligo/apis/CustomShare.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/apis/Download.py` & `aligo-6.0.4/src/aligo/apis/Download.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/apis/Drive.py` & `aligo-6.0.4/src/aligo/apis/Drive.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/apis/Duplicate.py` & `aligo-6.0.4/src/aligo/apis/Duplicate.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/apis/File.py` & `aligo-6.0.4/src/aligo/apis/File.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/apis/Move.py` & `aligo-6.0.4/src/aligo/apis/Move.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/apis/Other.py` & `aligo-6.0.4/src/aligo/apis/Other.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/apis/Recyclebin.py` & `aligo-6.0.4/src/aligo/apis/Recyclebin.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/apis/Search.py` & `aligo-6.0.4/src/aligo/apis/Search.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/apis/Share.py` & `aligo-6.0.4/src/aligo/apis/Share.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,98 +17,92 @@
 
 
 class Share(Core):
     """..."""
 
     def share_file(self,
                    file_id: str,
-                   share_name: str = None,
                    share_pwd: str = None,
                    expiration: str = None,
                    drive_id: str = None,
                    description: str = None) -> CreateShareLinkResponse:
         """
         官方：分享文件
         :param file_id: [必选] 文件id
-        :param share_name: [可选] 分享名称
         :param share_pwd: [可选] 分享密码，默认：None，表示无密码
         :param expiration: [可选] 有效期，utc时间字符串：YYYY-MM-DDTHH:mm:ss.SSSZ
         :param drive_id: [可选] 所属网盘id
         :param description: [可选] 描述
         :return: [CreateShareLinkResponse]
 
         用法示例：
         >>> from aligo import Aligo
         >>> ali = Aligo()
-        >>> share = ali.share_file('<file1_id>', share_name='share_name', share_pwd='2020', expiration='2021-12-01T00:00:00.000Z', description='description')
+        >>> share = ali.share_file('<file1_id>', share_pwd='2020', expiration='2021-12-01T00:00:00.000Z', description='description')
         >>> print(share)
         """
-        return self.share_files([file_id], share_name, share_pwd, expiration, drive_id, description)
+        return self.share_files([file_id], share_pwd, expiration, drive_id, description)
 
     def share_files(self,
                     file_id_list: List[str],
-                    share_name: str = None,
                     share_pwd: str = None,
                     expiration: str = None,
                     drive_id: str = None,
                     description: str = None) -> CreateShareLinkResponse:
         """
         官方：分享文件
         :param file_id_list: [必选] 文件id列表
-        :param share_name: [可选] 分享名称
         :param share_pwd: [可选] 分享密码，默认：None，表示无密码
         :param expiration: [可选] 有效期，utc时间字符串：YYYY-MM-DDTHH:mm:ss.SSSZ
         :param drive_id: [可选] 所属网盘id
         :param description: [可选] 描述
         :return: [CreateShareLinkResponse]
 
         用法示例：
         >>> from aligo import Aligo
         >>> ali = Aligo()
-        >>> share = ali.share_files(['<file1_id>','<file2_id>'], share_name='share_name', share_pwd='2020', expiration='2021-12-01T00:00:00.000Z', description='description')
+        >>> share = ali.share_files(['<file1_id>','<file2_id>'], share_pwd='2020', expiration='2021-12-01T00:00:00.000Z', description='description')
         >>> print(share)
         """
         body = CreateShareLinkRequest(
             file_id_list=file_id_list,
-            share_name=share_name,
             share_pwd=share_pwd,
             expiration=expiration,
             drive_id=drive_id,
             description=description,
         )
         return self._core_share_file(body)
 
-    def update_share(self,
-                     share_id: str,
-                     share_pwd: str = None,
-                     expiration: str = None,
-                     description: str = None,
-                     share_name: str = None) -> UpdateShareLinkResponse:
+    def update_share(
+            self,
+            share_id: str,
+            share_pwd: str = None,
+            expiration: str = None,
+            description: str = None,
+    ) -> UpdateShareLinkResponse:
         """
         官方：更新分享
         :param share_id: [必选] 分享id
         :param share_pwd: [可选] 分享密码，默认：None，表示无密码
         :param expiration: [可选] 有效期，utc时间字符串：YYYY-MM-DDTHH:mm:ss.SSSZ
         :param description: [可选] 描述
-        :param share_name: [可选] 分享名称
         :return: [UpdateShareLinkResponse]
 
         用法示例：
         >>> from aligo import Aligo
         >>> ali = Aligo()
-        >>> old_share = ali.share_file('<file_id>', share_name='old share')
-        >>> new_share = ali.update_share(old_share.share_id, share_name='new share')
+        >>> old_share = ali.share_file('<file_id>')
+        >>> new_share = ali.update_share(old_share.share_id)
         >>> print(new_share)
         """
         body = UpdateShareLinkRequest(
             share_id=share_id,
             share_pwd=share_pwd,
             expiration=expiration,
             description=description,
-            share_name=share_name,
         )
         return self._core_update_share(body)
 
     def cancel_share(self, share_id: str) -> CancelShareLinkResponse:
         """
         官方：取消分享
         :param share_id: [必选] 分享id
@@ -590,7 +584,22 @@
         """在分享中搜索文件"""
         _deprecation_warning(kwargs)
         if body is None:
             body = SearchShareFileRequest(share_id=share_token.share_id, keyword=keyword,
                                           order_by=f'{order_by} {order_direction}', **kwargs)
         result = self._core_search_share_files(body, share_token)
         return list(result)
+
+    def private_share_file(self, file_id: str, drive_id: str = None):
+        """APP 中的快传，有效期 24 小时，只能一个人保存"""
+        return self.private_share_files([file_id], drive_id)
+
+    def private_share_files(self, file_id_list: List[str], drive_id: str = None):
+        """APP 中的快传，有效期 24 小时，只能一个人保存"""
+        if drive_id is None:
+            drive_id = self.default_drive_id
+        return self._core_private_share_files(PrivateShareRequest(
+            drive_file_list=[
+                DriveFile(file_id=file_id, drive_id=drive_id)
+                for file_id in file_id_list
+            ]
+        ))
```

### Comparing `aligo-6.0.3/src/aligo/apis/Star.py` & `aligo-6.0.4/src/aligo/apis/Star.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/apis/SyncFolder.py` & `aligo-6.0.4/src/aligo/apis/SyncFolder.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/apis/Update.py` & `aligo-6.0.4/src/aligo/apis/Update.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/apis/Video.py` & `aligo-6.0.4/src/aligo/apis/Video.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/core/Album.py` & `aligo-6.0.4/src/aligo/core/Album.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/core/Auth.py` & `aligo-6.0.4/src/aligo/core/Auth.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/core/BaseAligo.py` & `aligo-6.0.4/src/aligo/core/BaseAligo.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/core/Compress.py` & `aligo-6.0.4/src/aligo/core/Compress.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/core/Config.py` & `aligo-6.0.4/src/aligo/core/Config.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,15 @@
 ADRIVE_V2_SHARE_LINK_GET_SHARE_BY_ANONYMOUS = '/adrive/v2/share_link/get_share_by_anonymous'
 V2_SHARE_LINK_GET_SHARE_TOKEN = '/v2/share_link/get_share_token'
 V2_FILE_GET_SHARE_LINK_DOWNLOAD_URL = '/v2/file/get_share_link_download_url'
 ADRIVE_V2_SHARE_LINK_EXTRACT_CODE = '/adrive/v2/share_link/extract_code'
 RECOMMEND_V1_SHARELINK_SEARCH = '/recommend/v1/shareLink/search'
 ADRIVE_V2_FILE_LIST_BY_SHARE = '/adrive/v2/file/list_by_share'
 ADRIVE_V2_FILE_GET_BY_SHARE = '/adrive/v2/file/get_by_share'
+ADRIVE_V1_SHARE_CREATE = '/adrive/v1/share/create'
 
 # 批量操作
 V3_BATCH = '/v3/batch'
 ADRIVE_V2_BATCH = '/adrive/v2/batch'
 
 # 福利码
 V1_USERS_REWARDS = '/v1/users/rewards'
```

### Comparing `aligo-6.0.3/src/aligo/core/Copy.py` & `aligo-6.0.4/src/aligo/core/Copy.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/core/Core.py` & `aligo-6.0.4/src/aligo/core/Core.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/core/Create.py` & `aligo-6.0.4/src/aligo/core/Create.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/core/Download.py` & `aligo-6.0.4/src/aligo/core/Download.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/core/Drive.py` & `aligo-6.0.4/src/aligo/core/Drive.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/core/Duplicate.py` & `aligo-6.0.4/src/aligo/core/Duplicate.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/core/EMail.py` & `aligo-6.0.4/src/aligo/core/EMail.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/core/File.py` & `aligo-6.0.4/src/aligo/core/File.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/core/LoginServer.py` & `aligo-6.0.4/src/aligo/core/LoginServer.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/core/Move.py` & `aligo-6.0.4/src/aligo/core/Move.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/core/Recyclebin.py` & `aligo-6.0.4/src/aligo/core/Recyclebin.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/core/Search.py` & `aligo-6.0.4/src/aligo/core/Search.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/core/Share.py` & `aligo-6.0.4/src/aligo/core/Share.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,7 +205,11 @@
         }
         eg: 'name match "epub"'
         eg: 'name match "epub" and category = "image"'
         category : BaseFileCategory
         """
         yield from self._list_file(
             RECOMMEND_V1_SHARELINK_SEARCH, body, SearchShareFileResponse, headers={'x-share-token': share_token})
+
+    def _core_private_share_files(self, body: PrivateShareRequest) -> PrivateShareResponse:
+        response = self._post(ADRIVE_V1_SHARE_CREATE, body=body)
+        return self._result(response, PrivateShareResponse)
```

### Comparing `aligo-6.0.3/src/aligo/core/Star.py` & `aligo-6.0.4/src/aligo/core/Star.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/core/Update.py` & `aligo-6.0.4/src/aligo/core/Update.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/core/User.py` & `aligo-6.0.4/src/aligo/core/User.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/core/Video.py` & `aligo-6.0.4/src/aligo/core/Video.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/request/AlbumListFilesRequest.py` & `aligo-6.0.4/src/aligo/request/AlbumListFilesRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/request/CreateFileRequest.py` & `aligo-6.0.4/src/aligo/request/CreateFileRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/request/CreateShareLinkRequest.py` & `aligo-6.0.4/src/aligo/request/CreateShareLinkRequest.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,15 +11,13 @@
 
     Attributes:
         drive_id (str):
         file_id_list (List[str]):
         share_pwd (str): 提取码，0-64个字符。长度0表示没有提取码。
         expiration (str): 失效时间点。RFC3339格式，比如："2020-06-28T11:33:00.000+08:00"。永久有效: ""
         description (str): 描述
-        share_name (str): 分享名，默认使用第一个文件名
     """
     drive_id: str = None
     file_id_list: List[str] = None
     share_pwd: str = None
     expiration: str = ''
     description: str = None
-    share_name: str = None
```

### Comparing `aligo-6.0.3/src/aligo/request/GetFileListRequest.py` & `aligo-6.0.4/src/aligo/request/GetFileListRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/request/GetFileRequest.py` & `aligo-6.0.4/src/aligo/request/GetFileRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/request/GetRecycleBinListRequest.py` & `aligo-6.0.4/src/aligo/request/GetRecycleBinListRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/request/GetShareFileListRequest.py` & `aligo-6.0.4/src/aligo/request/GetShareFileListRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/request/GetShareLinkDownloadUrlRequest.py` & `aligo-6.0.4/src/aligo/request/GetShareLinkDownloadUrlRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/request/GetShareLinkListRequest.py` & `aligo-6.0.4/src/aligo/request/GetShareLinkListRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/request/GetStarredListRequest.py` & `aligo-6.0.4/src/aligo/request/GetStarredListRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/request/SearchFileRequest.py` & `aligo-6.0.4/src/aligo/request/SearchFileRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/request/UpdateFileRequest.py` & `aligo-6.0.4/src/aligo/request/UpdateFileRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/request/UpdateShareLinkRequest.py` & `aligo-6.0.4/src/aligo/request/UpdateShareLinkRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,12 @@
     更新分享链接请求
 
     Attributes:
         share_id (str):
         share_pwd (str): 提取码，0-64个字符。长度0表示没有提取码。
         expiration (str): 失效时间点。RFC3339格式，比如："2020-06-28T11:33:00.000+08:00"。永久有效: ""
         description (str): 描述
-        share_name (str): 分享名，默认使用第一个文件名
     """
     share_id: str
     share_pwd: str = None
     expiration: str = ''
     description: str = None
-    share_name: str = None
```

### Comparing `aligo-6.0.3/src/aligo/request/__init__.py` & `aligo-6.0.4/src/aligo/request/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 from .GetStarredListRequest import GetStarredListRequest
 from .GetUploadUrlRequest import GetUploadUrlRequest
 from .GetVideoPlayInfoRequest import GetVideoPlayInfoRequest
 from .GetVideoPreviewPlayInfoRequest import GetVideoPreviewPlayInfoRequest
 from .ListToCleanRequest import ListToCleanRequest
 from .MoveFileRequest import MoveFileRequest
 from .MoveFileToTrashRequest import MoveFileToTrashRequest
+from .PrivateShareRequest import PrivateShareRequest
 from .RenameFileRequest import RenameFileRequest
 from .RestoreFileRequest import RestoreFileRequest
 from .SearchFileRequest import SearchFileRequest
 from .SearchShareFileRequest import SearchShareFileRequest
 from .ShareFileSaveToDriveRequest import ShareFileSaveToDriveRequest
 from .StarredFileRequest import StarredFileRequest
 from .TemplateRequest import TemplateRequest
```

### Comparing `aligo-6.0.3/src/aligo/response/CreateFileResponse.py` & `aligo-6.0.4/src/aligo/response/CreateFileResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/response/CreateShareLinkResponse.py` & `aligo-6.0.4/src/aligo/response/CreateShareLinkResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/response/DuplicateListResponse.py` & `aligo-6.0.4/src/aligo/response/DuplicateListResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/response/GetShareInfoResponse.py` & `aligo-6.0.4/src/aligo/response/GetShareInfoResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/response/GetShareTokenResponse.py` & `aligo-6.0.4/src/aligo/response/GetShareTokenResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/response/UpdateShareLinkResponse.py` & `aligo-6.0.4/src/aligo/response/UpdateShareLinkResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/response/__init__.py` & `aligo-6.0.4/src/aligo/response/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from .GetVideoPlayInfoResponse import GetVideoPlayInfoResponse
 from .GetVideoPreviewPlayInfoResponse import GetVideoPreviewPlayInfoResponse
 from .ListMyDrivesResponse import ListMyDrivesResponse
 from .ListResponse import ListResponse
 from .ListToCleanResponse import ListToCleanResponse
 from .MoveFileResponse import MoveFileResponse
 from .MoveFileToTrashResponse import MoveFileToTrashResponse
+from .PrivateShareResponse import PrivateShareResponse
 from .RestoreFileResponse import RestoreFileResponse
 from .RewardSpaceResponse import RewardSpaceResponse
 from .SearchFileResponse import SearchFileResponse
 from .SearchShareFileResponse import SearchShareFileResponse
 from .ShareFileSaveToDriveResponse import ShareFileSaveToDriveResponse
 from .ShareItemInfo import ShareItemInfo
 from .ShareLinkExtractCodeResponse import ShareLinkExtractCodeResponse
```

### Comparing `aligo-6.0.3/src/aligo/types/BaseAlbum.py` & `aligo-6.0.4/src/aligo/types/BaseAlbum.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/types/BaseDrive.py` & `aligo-6.0.4/src/aligo/types/BaseDrive.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/types/BaseFile.py` & `aligo-6.0.4/src/aligo/types/BaseFile.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/types/BaseShareFile.py` & `aligo-6.0.4/src/aligo/types/BaseShareFile.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/types/BaseUser.py` & `aligo-6.0.4/src/aligo/types/BaseUser.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/types/DataClass.py` & `aligo-6.0.4/src/aligo/types/DataClass.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/types/Enum.py` & `aligo-6.0.4/src/aligo/types/Enum.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/types/ImageMedia.py` & `aligo-6.0.4/src/aligo/types/ImageMedia.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/types/Null.py` & `aligo-6.0.4/src/aligo/types/Null.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/types/ShareLinkSchema.py` & `aligo-6.0.4/src/aligo/types/ShareLinkSchema.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/types/Token.py` & `aligo-6.0.4/src/aligo/types/Token.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/types/UserConfig.py` & `aligo-6.0.4/src/aligo/types/UserConfig.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/types/VideoMedia.py` & `aligo-6.0.4/src/aligo/types/VideoMedia.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/types/VideoPreview.py` & `aligo-6.0.4/src/aligo/types/VideoPreview.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/types/VideoPreviewPlayInfo.py` & `aligo-6.0.4/src/aligo/types/VideoPreviewPlayInfo.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.3/src/aligo/types/__init__.py` & `aligo-6.0.4/src/aligo/types/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from .BaseFile import BaseFile
 from .BaseShareFile import BaseShareFile
 from .BaseUser import BaseUser
 from .CroppingBoundary import CroppingBoundary
 from .CroppingSuggestionItem import CroppingSuggestionItem
 from .DataClass import DataClass
 from .DriveCapacityDetail import DriveCapacityDetail
+from .DriveFile import DriveFile
 from .EMailConfig import EMailConfig
 from .FaceThumbnail import FaceThumbnail
 from .FolderSizeInfo import FolderSizeInfo
 from .ImageMedia import ImageMedia
 from .ImageQuality import ImageQuality
 from .ImageTag import ImageTag
 from .ListAlbumItem import ListAlbumItem
```

### Comparing `aligo-6.0.3/src/aligo.egg-info/PKG-INFO` & `aligo-6.0.4/src/aligo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aligo
-Version: 6.0.3
+Version: 6.0.4
 Summary: aliyun drive sdk
 Author: foyoux
 Project-URL: Source, https://github.com/foyoux/aligo
 Project-URL: Homepage, https://github.com/foyoux/aligo
 Project-URL: Bug Tracker, https://github.com/foyoux/aligo/issues
 Keywords: aligo
 Classifier: Programming Language :: Python
```

### Comparing `aligo-6.0.3/src/aligo.egg-info/SOURCES.txt` & `aligo-6.0.4/src/aligo.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -95,14 +95,15 @@
 src/aligo/request/GetStarredListRequest.py
 src/aligo/request/GetUploadUrlRequest.py
 src/aligo/request/GetVideoPlayInfoRequest.py
 src/aligo/request/GetVideoPreviewPlayInfoRequest.py
 src/aligo/request/ListToCleanRequest.py
 src/aligo/request/MoveFileRequest.py
 src/aligo/request/MoveFileToTrashRequest.py
+src/aligo/request/PrivateShareRequest.py
 src/aligo/request/RenameFileRequest.py
 src/aligo/request/RestoreFileRequest.py
 src/aligo/request/SearchFileRequest.py
 src/aligo/request/SearchShareFileRequest.py
 src/aligo/request/ShareFileSaveToDriveRequest.py
 src/aligo/request/StarredFileRequest.py
 src/aligo/request/TemplateRequest.py
@@ -139,14 +140,15 @@
 src/aligo/response/GetVideoPlayInfoResponse.py
 src/aligo/response/GetVideoPreviewPlayInfoResponse.py
 src/aligo/response/ListMyDrivesResponse.py
 src/aligo/response/ListResponse.py
 src/aligo/response/ListToCleanResponse.py
 src/aligo/response/MoveFileResponse.py
 src/aligo/response/MoveFileToTrashResponse.py
+src/aligo/response/PrivateShareResponse.py
 src/aligo/response/RestoreFileResponse.py
 src/aligo/response/RewardSpaceResponse.py
 src/aligo/response/SearchFileResponse.py
 src/aligo/response/SearchShareFileResponse.py
 src/aligo/response/ShareFileSaveToDriveResponse.py
 src/aligo/response/ShareItemInfo.py
 src/aligo/response/ShareLinkExtractCodeResponse.py
@@ -162,14 +164,15 @@
 src/aligo/types/BaseFile.py
 src/aligo/types/BaseShareFile.py
 src/aligo/types/BaseUser.py
 src/aligo/types/CroppingBoundary.py
 src/aligo/types/CroppingSuggestionItem.py
 src/aligo/types/DataClass.py
 src/aligo/types/DriveCapacityDetail.py
+src/aligo/types/DriveFile.py
 src/aligo/types/EMailConfig.py
 src/aligo/types/Enum.py
 src/aligo/types/FaceThumbnail.py
 src/aligo/types/FieldsInfo.py
 src/aligo/types/FolderSizeInfo.py
 src/aligo/types/ImageMedia.py
 src/aligo/types/ImageQuality.py
```

