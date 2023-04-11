# Comparing `tmp/nerualpha-4.1.0rc4.tar.gz` & `tmp/nerualpha-4.1.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nerualpha-4.1.0rc4.tar", max compression
+gzip compressed data, was "nerualpha-4.1.0rc5.tar", max compression
```

## Comparing `nerualpha-4.1.0rc4.tar` & `nerualpha-4.1.0rc5.tar`

### file list

```diff
@@ -1,445 +1,446 @@
--rw-r--r--   0        0        0      594 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/README.md
--rw-r--r--   0        0        0      843 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/pyproject.toml
--rw-r--r--   0        0        0     1708 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/IBridge.py
--rw-r--r--   0        0        0      853 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/INeru.py
--rw-r--r--   0        0        0        0 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/__init__.py
--rw-r--r--   0        0        0     4323 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/bridge.py
--rw-r--r--   0        0        0     3926 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/neru.py
--rw-r--r--   0        0        0        0 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/__init__.py
--rw-r--r--   0        0        0     1310 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/assets/IAssets.py
--rw-r--r--   0        0        0        0 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/assets/__init__.py
--rw-r--r--   0        0        0     5788 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/assets/assets.py
--rw-r--r--   0        0        0      316 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/assets/assetsActions.py
--rw-r--r--   0        0        0        0 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/assets/contracts/__init__.py
--rw-r--r--   0        0        0     1112 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/assets/contracts/assetInfo.py
--rw-r--r--   0        0        0     1083 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/assets/contracts/assetLinkResponse.py
--rw-r--r--   0        0        0     1149 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/assets/contracts/assetListResponse.py
--rw-r--r--   0        0        0     1100 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/assets/contracts/directoryPayload.py
--rw-r--r--   0        0        0     1087 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/assets/contracts/getAssetPayload.py
--rw-r--r--   0        0        0     1098 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/assets/contracts/getAssetResponse.py
--rw-r--r--   0        0        0     1145 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/assets/contracts/linkPayload.py
--rw-r--r--   0        0        0     1212 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/assets/contracts/listAssetsPayload.py
--rw-r--r--   0        0        0     1165 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/assets/contracts/removeAssetPayload.py
--rw-r--r--   0        0        0      304 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/events/IEventEmitter.py
--rw-r--r--   0        0        0      312 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/events/IEventFactory.py
--rw-r--r--   0        0        0      388 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/events/INeruEvent.py
--rw-r--r--   0        0        0      200 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/events/ISessionCreatedDetails.py
--rw-r--r--   0        0        0        0 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/events/__init__.py
--rw-r--r--   0        0        0     2804 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/events/eventEmitter.py
--rw-r--r--   0        0        0     2389 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/events/eventFactory.py
--rw-r--r--   0        0        0     1348 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/events/neruEvent.py
--rw-r--r--   0        0        0      189 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/events/neruEventSourceTypes.py
--rw-r--r--   0        0        0      477 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/events/neruEventTypes.py
--rw-r--r--   0        0        0     1224 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/events/sessionCreatedDetails.py
--rw-r--r--   0        0        0      447 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/logger/ILogAction.py
--rw-r--r--   0        0        0      221 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/logger/ILogContext.py
--rw-r--r--   0        0        0      311 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/logger/ILogger.py
--rw-r--r--   0        0        0        0 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/logger/__init__.py
--rw-r--r--   0        0        0     1415 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/logger/logAction.py
--rw-r--r--   0        0        0     1292 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/logger/logContext.py
--rw-r--r--   0        0        0      228 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/logger/logLevels.py
--rw-r--r--   0        0        0     2990 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/logger/logger.py
--rw-r--r--   0        0        0      212 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/logger/sourceTypes.py
--rw-r--r--   0        0        0        0 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/meetings/__init__.py
--rw-r--r--   0        0        0      199 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/meetings/contracts/ICreateRoomPayload.py
--rw-r--r--   0        0        0        0 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/meetings/contracts/__init__.py
--rw-r--r--   0        0        0     1667 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/meetings/contracts/createRoomPayload.py
--rw-r--r--   0        0        0     1055 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/meetings/contracts/deleteRoomPayload.py
--rw-r--r--   0        0        0     1274 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/meetings/contracts/getRoomsResponse.py
--rw-r--r--   0        0        0     1194 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/meetings/contracts/pageLinks.py
--rw-r--r--   0        0        0     1111 2023-04-05 11:48:05.932851 nerualpha-4.1.0rc4/src/nerualpha/providers/meetings/contracts/recordingOptions.py
--rw-r--r--   0        0        0     1158 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/meetings/contracts/roomLinks.py
--rw-r--r--   0        0        0     1465 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/meetings/contracts/roomResponse.py
--rw-r--r--   0        0        0     1158 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/meetings/contracts/roomsEmbedded.py
--rw-r--r--   0        0        0     1208 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/meetings/contracts/updateRoomDetails.py
--rw-r--r--   0        0        0     1232 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/meetings/contracts/updateRoomPayload.py
--rw-r--r--   0        0        0     3288 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/meetings/meetings.py
--rw-r--r--   0        0        0      203 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/meetings/roomTypes.py
--rw-r--r--   0        0        0     1596 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/IMessages.py
--rw-r--r--   0        0        0        0 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/__init__.py
--rw-r--r--   0        0        0      234 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/IBaseMessage.py
--rw-r--r--   0        0        0      198 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/IImageData.py
--rw-r--r--   0        0        0      495 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/IListenEventsPayload.py
--rw-r--r--   0        0        0      497 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/IListenMessagesPayload.py
--rw-r--r--   0        0        0      359 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/IMMSAudioMessage.py
--rw-r--r--   0        0        0      359 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/IMMSImageMessage.py
--rw-r--r--   0        0        0      359 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/IMMSVCardMessage.py
--rw-r--r--   0        0        0      359 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/IMMSVideoMessage.py
--rw-r--r--   0        0        0      215 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/IMessageContact.py
--rw-r--r--   0        0        0      199 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/IMessenger.py
--rw-r--r--   0        0        0      365 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/IMessengerAudioMessage.py
--rw-r--r--   0        0        0      363 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/IMessengerFileMessage.py
--rw-r--r--   0        0        0      365 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/IMessengerImageMessage.py
--rw-r--r--   0        0        0      194 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/IMessengerTextMessage.py
--rw-r--r--   0        0        0      365 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/IMessengerVideoMessage.py
--rw-r--r--   0        0        0      270 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/ISMSMessage.py
--rw-r--r--   0        0        0      285 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/ISendImageContent.py
--rw-r--r--   0        0        0      294 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/ISendImageMessage.py
--rw-r--r--   0        0        0      426 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/ISendImagePayload.py
--rw-r--r--   0        0        0      276 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/ISendImageResponse.py
--rw-r--r--   0        0        0      194 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/ISendResponse.py
--rw-r--r--   0        0        0      203 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/ISendTextContent.py
--rw-r--r--   0        0        0      297 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/ISendTextMessagePayload.py
--rw-r--r--   0        0        0      443 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/ISendTextPayload.py
--rw-r--r--   0        0        0      199 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/IURLPayload.py
--rw-r--r--   0        0        0      196 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/IUnsubscribeEventsPayload.py
--rw-r--r--   0        0        0      361 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/IViberImageMessage.py
--rw-r--r--   0        0        0      216 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/IViberService.py
--rw-r--r--   0        0        0      276 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/IViberTextMessage.py
--rw-r--r--   0        0        0      199 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/IWhatsapp.py
--rw-r--r--   0        0        0      364 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/IWhatsappAudioMessage.py
--rw-r--r--   0        0        0      362 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/IWhatsappFileMessage.py
--rw-r--r--   0        0        0      364 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/IWhatsappImageMessage.py
--rw-r--r--   0        0        0      215 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/IWhatsappTemplate.py
--rw-r--r--   0        0        0      482 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/IWhatsappTemplateMessage.py
--rw-r--r--   0        0        0      279 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/IWhatsappTextMessage.py
--rw-r--r--   0        0        0      364 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/IWhatsappVideoMessage.py
--rw-r--r--   0        0        0        0 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/__init__.py
--rw-r--r--   0        0        0     1206 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/baseMessage.py
--rw-r--r--   0        0        0     1220 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/imageData.py
--rw-r--r--   0        0        0     1492 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/listenEventsPayload.py
--rw-r--r--   0        0        0     1500 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/listenMessagesPayload.py
--rw-r--r--   0        0        0     1202 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/messageContact.py
--rw-r--r--   0        0        0     1508 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/messengerAudioMessage.py
--rw-r--r--   0        0        0     1502 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/messengerFileMessage.py
--rw-r--r--   0        0        0     1508 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/messengerImageMessage.py
--rw-r--r--   0        0        0     1419 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/messengerTextMessage.py
--rw-r--r--   0        0        0     1508 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/messengerVideoMessage.py
--rw-r--r--   0        0        0     1385 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/mmsAudioMessage.py
--rw-r--r--   0        0        0     1372 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/mmsImageMessage.py
--rw-r--r--   0        0        0     1372 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/mmsVCardMessage.py
--rw-r--r--   0        0        0     1372 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/mmsVideoMessage.py
--rw-r--r--   0        0        0     1330 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/sendImageContent.py
--rw-r--r--   0        0        0     1309 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/sendImageMessage.py
--rw-r--r--   0        0        0     1679 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/sendImagePayload.py
--rw-r--r--   0        0        0     1166 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/sendResponse.py
--rw-r--r--   0        0        0     1235 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/sendTextContent.py
--rw-r--r--   0        0        0     1330 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/sendTextMessagePayload.py
--rw-r--r--   0        0        0     1729 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/sendTextPayload.py
--rw-r--r--   0        0        0     1267 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/smsMessage.py
--rw-r--r--   0        0        0     1220 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/unsubscribeEventsPayload.py
--rw-r--r--   0        0        0     1173 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/urlPayload.py
--rw-r--r--   0        0        0     1509 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/viberImageMessage.py
--rw-r--r--   0        0        0     1420 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/viberTextMessage.py
--rw-r--r--   0        0        0     1397 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/whatsappAudioMessage.py
--rw-r--r--   0        0        0     1391 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/whatsappFileMessage.py
--rw-r--r--   0        0        0     1397 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/whatsappImageMessage.py
--rw-r--r--   0        0        0     1528 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/whatsappTemplateMessage.py
--rw-r--r--   0        0        0     1308 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/whatsappTextMessage.py
--rw-r--r--   0        0        0     1397 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/whatsappVideoMessage.py
--rw-r--r--   0        0        0      317 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/messageActions.py
--rw-r--r--   0        0        0      219 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/messageChannelType.py
--rw-r--r--   0        0        0      298 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/messageType.py
--rw-r--r--   0        0        0     4786 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/messages/messages.py
--rw-r--r--   0        0        0        0 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/numbers/__init__.py
--rw-r--r--   0        0        0      187 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/numbers/contracts/IBaseNumberOptions.py
--rw-r--r--   0        0        0      411 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/numbers/contracts/IGetNumbersOptions.py
--rw-r--r--   0        0        0      331 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/numbers/contracts/INumberOptions.py
--rw-r--r--   0        0        0      403 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/numbers/contracts/ISearchNumbersOptions.py
--rw-r--r--   0        0        0      450 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/numbers/contracts/IUpdateNumberOptions.py
--rw-r--r--   0        0        0        0 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/numbers/contracts/__init__.py
--rw-r--r--   0        0        0     1163 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/numbers/contracts/baseNumberOptions.py
--rw-r--r--   0        0        0     1453 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/numbers/contracts/getNumbersOptions.py
--rw-r--r--   0        0        0     1185 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/numbers/contracts/getNumbersResponse.py
--rw-r--r--   0        0        0     1315 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/numbers/contracts/numberOptions.py
--rw-r--r--   0        0        0     1259 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/numbers/contracts/numberResponse.py
--rw-r--r--   0        0        0     1129 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/numbers/contracts/numbersOperationResponse.py
--rw-r--r--   0        0        0     1515 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/numbers/contracts/searchNumbersOptions.py
--rw-r--r--   0        0        0     1492 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/numbers/contracts/updateNumberOptions.py
--rw-r--r--   0        0        0      208 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/numbers/numberFeature.py
--rw-r--r--   0        0        0     7697 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/numbers/numbers.py
--rw-r--r--   0        0        0     1527 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/queue/IQueue.py
--rw-r--r--   0        0        0        0 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/queue/__init__.py
--rw-r--r--   0        0        0      236 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/queue/contracts/ICreateQueueOptions.py
--rw-r--r--   0        0        0      392 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/queue/contracts/ICreateQueuePayload.py
--rw-r--r--   0        0        0      386 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/queue/contracts/IQueueDetails.py
--rw-r--r--   0        0        0      280 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/queue/contracts/IQueueDetailsStats.py
--rw-r--r--   0        0        0      211 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/queue/contracts/IQueueRate.py
--rw-r--r--   0        0        0      220 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/queue/contracts/IUpdateQueueOptions.py
--rw-r--r--   0        0        0      269 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/queue/contracts/IUpdateQueuePayload.py
--rw-r--r--   0        0        0        0 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/queue/contracts/__init__.py
--rw-r--r--   0        0        0     1225 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/queue/contracts/createQueueOptions.py
--rw-r--r--   0        0        0     1382 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/queue/contracts/createQueuePayload.py
--rw-r--r--   0        0        0      402 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/queue/contracts/queueDetailsResponse.py
--rw-r--r--   0        0        0     1172 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/queue/contracts/queueRate.py
--rw-r--r--   0        0        0     1208 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/queue/contracts/updateQueueOptions.py
--rw-r--r--   0        0        0     1256 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/queue/contracts/updateQueuePayload.py
--rw-r--r--   0        0        0     6091 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/queue/queue.py
--rw-r--r--   0        0        0     1044 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/scheduler/IScheduler.py
--rw-r--r--   0        0        0        0 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/scheduler/__init__.py
--rw-r--r--   0        0        0      289 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/scheduler/contracts/IIntervalParams.py
--rw-r--r--   0        0        0      208 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/scheduler/contracts/IListAllPayload.py
--rw-r--r--   0        0        0      187 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/scheduler/contracts/ISchedulePayload.py
--rw-r--r--   0        0        0      374 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/scheduler/contracts/IStartAtParams.py
--rw-r--r--   0        0        0      447 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/scheduler/contracts/IStartAtPayload.py
--rw-r--r--   0        0        0      208 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/scheduler/contracts/IUntilParams.py
--rw-r--r--   0        0        0        0 2023-04-05 11:48:05.936852 nerualpha-4.1.0rc4/src/nerualpha/providers/scheduler/contracts/__init__.py
--rw-r--r--   0        0        0     1381 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/scheduler/contracts/getSchedulerResponse.py
--rw-r--r--   0        0        0     1269 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/scheduler/contracts/intervalParams.py
--rw-r--r--   0        0        0     1305 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/scheduler/contracts/listAllPayload.py
--rw-r--r--   0        0        0     1123 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/scheduler/contracts/listAllSchedulersResponse.py
--rw-r--r--   0        0        0     1138 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/scheduler/contracts/schedulerExecutionInfo.py
--rw-r--r--   0        0        0     1186 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/scheduler/contracts/schedulerPayload.py
--rw-r--r--   0        0        0     1375 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/scheduler/contracts/startAtParams.py
--rw-r--r--   0        0        0     1456 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/scheduler/contracts/startAtPayload.py
--rw-r--r--   0        0        0     1179 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/scheduler/contracts/untilParams.py
--rw-r--r--   0        0        0     3999 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/scheduler/scheduler.py
--rw-r--r--   0        0        0      237 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/scheduler/schedulerActions.py
--rw-r--r--   0        0        0     1971 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/state/IState.py
--rw-r--r--   0        0        0      240 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/state/IStateCommand.py
--rw-r--r--   0        0        0        0 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/state/__init__.py
--rw-r--r--   0        0        0      212 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/state/expireOptions.py
--rw-r--r--   0        0        0     9864 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/state/state.py
--rw-r--r--   0        0        0     1341 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/state/stateCommand.py
--rw-r--r--   0        0        0      694 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/state/stateOperations.py
--rw-r--r--   0        0        0     4370 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/IConversation.py
--rw-r--r--   0        0        0     1208 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/IUsers.py
--rw-r--r--   0        0        0     1636 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/IVoice.py
--rw-r--r--   0        0        0        0 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/__init__.py
--rw-r--r--   0        0        0      207 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/callDirections.py
--rw-r--r--   0        0        0      257 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/callStatuses.py
--rw-r--r--   0        0        0      344 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/IAcceptInboundCallBody.py
--rw-r--r--   0        0        0      215 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/IAcceptInboundCallEndpoint.py
--rw-r--r--   0        0        0      403 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/IAcceptInboundCallEvent.py
--rw-r--r--   0        0        0      460 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/IAcceptInboundCallPayload.py
--rw-r--r--   0        0        0      209 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/IAddUserPayload.py
--rw-r--r--   0        0        0      225 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/IAudioSettings.py
--rw-r--r--   0        0        0      536 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/IChannel.py
--rw-r--r--   0        0        0      190 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/IChannelEndpoint.py
--rw-r--r--   0        0        0      291 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/IChannelPhoneEndpoint.py
--rw-r--r--   0        0        0      346 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/IChannelSIPEndpoint.py
--rw-r--r--   0        0        0      292 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/IChannelVBCEndpoint.py
--rw-r--r--   0        0        0      304 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/IConversationPayloadWithCallback.py
--rw-r--r--   0        0        0      220 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/ICreateConversationPayload.py
--rw-r--r--   0        0        0      250 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/ICreateUserPayload.py
--rw-r--r--   0        0        0      277 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/IDeleteMemberPayload.py
--rw-r--r--   0        0        0      214 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/IEarmuffPayload.py
--rw-r--r--   0        0        0      371 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/IInviteMemberPayload.py
--rw-r--r--   0        0        0      179 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/ILeg.py
--rw-r--r--   0        0        0      293 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/IMedia.py
--rw-r--r--   0        0        0      211 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/IMutePayload.py
--rw-r--r--   0        0        0      423 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/IOnInboundCallPayload.py
--rw-r--r--   0        0        0      189 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/IPlayStopBody.py
--rw-r--r--   0        0        0      300 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/IPlayStopPayload.py
--rw-r--r--   0        0        0      241 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/IPlayStreamBody.py
--rw-r--r--   0        0        0      308 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/IPlayStreamPayload.py
--rw-r--r--   0        0        0      193 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/IReason.py
--rw-r--r--   0        0        0      187 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/ISayStopBody.py
--rw-r--r--   0        0        0      296 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/ISayStopPayload.py
--rw-r--r--   0        0        0      291 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/ISayTextBody.py
--rw-r--r--   0        0        0      293 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/ISayTextParams.py
--rw-r--r--   0        0        0      285 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/ISayTextPayload.py
--rw-r--r--   0        0        0      373 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/ITransferMemberPayload.py
--rw-r--r--   0        0        0      250 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/IUpdateUserPayload.py
--rw-r--r--   0        0        0      251 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/IUser.py
--rw-r--r--   0        0        0      277 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/IVapiAnswerCallBack.py
--rw-r--r--   0        0        0      274 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/IVapiCreateCallOptions.py
--rw-r--r--   0        0        0      373 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/IVapiCreateCallPayload.py
--rw-r--r--   0        0        0      312 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/IVapiEventCallBackPayload.py
--rw-r--r--   0        0        0      233 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/IVapiEventParams.py
--rw-r--r--   0        0        0     1063 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/Link.py
--rw-r--r--   0        0        0        0 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/__init__.py
--rw-r--r--   0        0        0     1341 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/acceptInboundCallBody.py
--rw-r--r--   0        0        0     1224 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/acceptInboundCallEndpoint.py
--rw-r--r--   0        0        0     1407 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/acceptInboundCallEvent.py
--rw-r--r--   0        0        0     1824 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/acceptInboundCallPayload.py
--rw-r--r--   0        0        0     1240 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/addUserPayload.py
--rw-r--r--   0        0        0     1351 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/addUserResponse.py
--rw-r--r--   0        0        0     1261 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/audioSayResponseBody.py
--rw-r--r--   0        0        0     1078 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/audioSayStopResponseBody.py
--rw-r--r--   0        0        0     1308 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/audioSettings.py
--rw-r--r--   0        0        0     1605 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/channel.py
--rw-r--r--   0        0        0     1315 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/channelAppEndpoint.py
--rw-r--r--   0        0        0     1342 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/channelPhoneEndpoint.py
--rw-r--r--   0        0        0     1626 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/channelSIPEndpoint.py
--rw-r--r--   0        0        0     1344 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/channelVBCEndpoint.py
--rw-r--r--   0        0        0     1430 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/conversationPayloadWithCallback.py
--rw-r--r--   0        0        0     1133 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/conversationTimestamp.py
--rw-r--r--   0        0        0     1303 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/createConversationPayload.py
--rw-r--r--   0        0        0     1522 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/createConversationResponse.py
--rw-r--r--   0        0        0     1428 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/createUserPayload.py
--rw-r--r--   0        0        0     1399 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/deleteMemberPayload.py
--rw-r--r--   0        0        0     1501 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/earmuffPayload.py
--rw-r--r--   0        0        0     1073 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/earmuffResponseBody.py
--rw-r--r--   0        0        0     1152 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/embeddedUsers.py
--rw-r--r--   0        0        0     1229 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/eventEmbedded.py
--rw-r--r--   0        0        0     1396 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/eventResponse.py
--rw-r--r--   0        0        0     1271 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/getUsersResponse.py
--rw-r--r--   0        0        0     1751 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/inviteMemberPayload.py
--rw-r--r--   0        0        0     1121 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/leg.py
--rw-r--r--   0        0        0     1315 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/media.py
--rw-r--r--   0        0        0     1063 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/member.py
--rw-r--r--   0        0        0     1570 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/memberResponse.py
--rw-r--r--   0        0        0     1121 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/memberTimestamp.py
--rw-r--r--   0        0        0     1483 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/mutePayload.py
--rw-r--r--   0        0        0     1070 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/muteResponseBody.py
--rw-r--r--   0        0        0     1571 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/onInboundCallPayload.py
--rw-r--r--   0        0        0     1187 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/playStopBody.py
--rw-r--r--   0        0        0     1572 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/playStopPayload.py
--rw-r--r--   0        0        0     1226 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/playStreamBody.py
--rw-r--r--   0        0        0     1490 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/playStreamPayload.py
--rw-r--r--   0        0        0     1155 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/playStreamResponseBody.py
--rw-r--r--   0        0        0     1081 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/playStreamStopResponseBody.py
--rw-r--r--   0        0        0     1197 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/reason.py
--rw-r--r--   0        0        0     1122 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/responseProperties.py
--rw-r--r--   0        0        0     1179 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/sayStopBody.py
--rw-r--r--   0        0        0     1559 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/sayStopPayload.py
--rw-r--r--   0        0        0     1313 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/sayTextBody.py
--rw-r--r--   0        0        0     1321 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/sayTextParams.py
--rw-r--r--   0        0        0     1468 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/sayTextPayload.py
--rw-r--r--   0        0        0     1126 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/selfLink.py
--rw-r--r--   0        0        0     1966 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/transferMemberPayload.py
--rw-r--r--   0        0        0     1456 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/updateUserPayload.py
--rw-r--r--   0        0        0     1235 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/user.py
--rw-r--r--   0        0        0     1123 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/userEmbedded.py
--rw-r--r--   0        0        0     1453 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/userResponse.py
--rw-r--r--   0        0        0     1184 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/userSummary.py
--rw-r--r--   0        0        0     1125 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/userTimestamp.py
--rw-r--r--   0        0        0     1294 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/vapiAnswerCallBack.py
--rw-r--r--   0        0        0     1301 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/vapiCreateCallOptions.py
--rw-r--r--   0        0        0     2231 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/vapiCreateCallPayload.py
--rw-r--r--   0        0        0     1136 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/vapiCreateCallResponse.py
--rw-r--r--   0        0        0     1338 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/vapiEventCallBackPayload.py
--rw-r--r--   0        0        0     1227 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/vapiEventParams.py
--rw-r--r--   0        0        0    11681 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/conversation.py
--rw-r--r--   0        0        0      253 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/csChannelTypes.py
--rw-r--r--   0        0        0      743 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/csEvents.py
--rw-r--r--   0        0        0      174 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/memberActions.py
--rw-r--r--   0        0        0      243 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/memberStates.py
--rw-r--r--   0        0        0     3730 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/users.py
--rw-r--r--   0        0        0     7104 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/voice.py
--rw-r--r--   0        0        0      405 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/voice/voiceActions.py
--rw-r--r--   0        0        0      414 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/vonageAI/IVonageAI.py
--rw-r--r--   0        0        0        0 2023-04-05 11:48:05.940852 nerualpha-4.1.0rc4/src/nerualpha/providers/vonageAI/__init__.py
--rw-r--r--   0        0        0      193 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/providers/vonageAI/contracts/IImportPayload.py
--rw-r--r--   0        0        0      288 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/providers/vonageAI/contracts/IVonageAiAnalyzePayload.py
--rw-r--r--   0        0        0      384 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/providers/vonageAI/contracts/IVonageAiImportModelPayload.py
--rw-r--r--   0        0        0        0 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/providers/vonageAI/contracts/__init__.py
--rw-r--r--   0        0        0     1208 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/providers/vonageAI/contracts/importPayload.py
--rw-r--r--   0        0        0     1369 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/providers/vonageAI/contracts/vonageAiAnalyzePayload.py
--rw-r--r--   0        0        0     1489 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/providers/vonageAI/contracts/vonageAiImportModelPayload.py
--rw-r--r--   0        0        0     2513 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/providers/vonageAI/vonageAI.py
--rw-r--r--   0        0        0      209 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/providers/vonageAI/vonageAIActions.py
--rw-r--r--   0        0        0      385 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/providers/vonageAPI/IVonageAPI.py
--rw-r--r--   0        0        0        0 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/providers/vonageAPI/__init__.py
--rw-r--r--   0        0        0      241 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/providers/vonageAPI/contracts/IInvokePayload.py
--rw-r--r--   0        0        0        0 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/providers/vonageAPI/contracts/__init__.py
--rw-r--r--   0        0        0     1304 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/providers/vonageAPI/contracts/invokePayload.py
--rw-r--r--   0        0        0     1775 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/providers/vonageAPI/vonageAPI.py
--rw-r--r--   0        0        0      181 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/providers/vonageAPI/vonageAPIActions.py
--rw-r--r--   0        0        0      222 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/request/IFormDataObject.py
--rw-r--r--   0        0        0      194 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/request/IRequest.py
--rw-r--r--   0        0        0      356 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/request/IRequestParams.py
--rw-r--r--   0        0        0        0 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/request/__init__.py
--rw-r--r--   0        0        0     1181 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/request/formDataObject.py
--rw-r--r--   0        0        0     1130 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/request/request.py
--rw-r--r--   0        0        0      288 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/request/requestMethods.py
--rw-r--r--   0        0        0     1335 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/request/requestParams.py
--rw-r--r--   0        0        0      264 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/request/responseTypes.py
--rw-r--r--   0        0        0        0 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/services/__init__.py
--rw-r--r--   0        0        0      276 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/services/commandService/ICommandService.py
--rw-r--r--   0        0        0        0 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/services/commandService/__init__.py
--rw-r--r--   0        0        0     1697 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/services/commandService/commandService.py
--rw-r--r--   0        0        0      551 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/services/config/IConfig.py
--rw-r--r--   0        0        0      234 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/services/config/IPathObject.py
--rw-r--r--   0        0        0        0 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/services/config/__init__.py
--rw-r--r--   0        0        0     3902 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/services/config/config.py
--rw-r--r--   0        0        0     1191 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/services/config/pathObject.py
--rw-r--r--   0        0        0      201 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/services/jwt/IAcl.py
--rw-r--r--   0        0        0      242 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/services/jwt/ICreateVonageTokenParams.py
--rw-r--r--   0        0        0      437 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/services/jwt/IJwt.py
--rw-r--r--   0        0        0        0 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/services/jwt/__init__.py
--rw-r--r--   0        0        0     1130 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/services/jwt/acl.py
--rw-r--r--   0        0        0     1247 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/services/jwt/createVonageTokenParams.py
--rw-r--r--   0        0        0     3103 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/services/jwt/jwt.py
--rw-r--r--   0        0        0     1224 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/services/jwt/neruJWTPayload.py
--rw-r--r--   0        0        0     1203 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/services/jwt/vonageJWTPayload.py
--rw-r--r--   0        0        0      405 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/session/IActionPayload.py
--rw-r--r--   0        0        0      318 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/session/ICommand.py
--rw-r--r--   0        0        0      212 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/session/IFilter.py
--rw-r--r--   0        0        0      274 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/session/IPayloadWithCallback.py
--rw-r--r--   0        0        0      281 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/session/IRequestInterface.py
--rw-r--r--   0        0        0     1203 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/session/ISession.py
--rw-r--r--   0        0        0      337 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/session/IWrappedCallback.py
--rw-r--r--   0        0        0        0 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/session/__init__.py
--rw-r--r--   0        0        0     1601 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/session/actionPayload.py
--rw-r--r--   0        0        0     1324 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/session/command.py
--rw-r--r--   0        0        0     1229 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/session/filter.py
--rw-r--r--   0        0        0     5721 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/session/neruSession.py
--rw-r--r--   0        0        0     1280 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/session/payloadWithCallback.py
--rw-r--r--   0        0        0     1827 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/session/requestInterface.py
--rw-r--r--   0        0        0     1665 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/session/requestInterfaceForCallbacks.py
--rw-r--r--   0        0        0     1541 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/session/requestInterfaceWithParams.py
--rw-r--r--   0        0        0     1302 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/session/wrappedCallback.py
--rw-r--r--   0        0        0        0 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/smokes/__init__.py
--rw-r--r--   0        0        0     2180 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/smokes/assetsTest.py
--rw-r--r--   0        0        0     4230 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/smokes/messagesTest.py
--rw-r--r--   0        0        0     3884 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/smokes/schedulerTest.py
--rw-r--r--   0        0        0     1106 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/smokes/schedulerTestPayload.py
--rw-r--r--   0        0        0     2734 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/smokes/stateTest.py
--rw-r--r--   0        0        0     3983 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/smokes/voiceTest.py
--rw-r--r--   0        0        0      250 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/IBaseEvent.py
--rw-r--r--   0        0        0      183 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/IUrlPayload.py
--rw-r--r--   0        0        0        0 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/__init__.py
--rw-r--r--   0        0        0     1202 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/baseEvent.py
--rw-r--r--   0        0        0      261 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/messenger/IMessangerEvent.py
--rw-r--r--   0        0        0      352 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/messenger/IMessengerAudioEvent.py
--rw-r--r--   0        0        0      350 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/messenger/IMessengerFileEvent.py
--rw-r--r--   0        0        0      352 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/messenger/IMessengerImageEvent.py
--rw-r--r--   0        0        0      282 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/messenger/IMessengerTextEvent.py
--rw-r--r--   0        0        0      285 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/messenger/IMessengerUnsupportedEvent.py
--rw-r--r--   0        0        0      352 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/messenger/IMessengerVideoEvent.py
--rw-r--r--   0        0        0        0 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/messenger/__init__.py
--rw-r--r--   0        0        0     1357 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/messenger/messengerAudioEvent.py
--rw-r--r--   0        0        0     1254 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/messenger/messengerEvent.py
--rw-r--r--   0        0        0     1352 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/messenger/messengerFileEvent.py
--rw-r--r--   0        0        0     1357 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/messenger/messengerImageEvent.py
--rw-r--r--   0        0        0     1284 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/messenger/messengerTextEvent.py
--rw-r--r--   0        0        0     1298 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/messenger/messengerUnsupportedEvent.py
--rw-r--r--   0        0        0     1357 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/messenger/messengerVideoEvent.py
--rw-r--r--   0        0        0      322 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/mms/IMMSAudioEvent.py
--rw-r--r--   0        0        0      255 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/mms/IMMSEvent.py
--rw-r--r--   0        0        0      322 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/mms/IMMSImageEvent.py
--rw-r--r--   0        0        0      322 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/mms/IMMSVCardEvent.py
--rw-r--r--   0        0        0      322 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/mms/IMMSVideoEvent.py
--rw-r--r--   0        0        0        0 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/mms/__init__.py
--rw-r--r--   0        0        0     1327 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/mms/mmsAudioEvent.py
--rw-r--r--   0        0        0     1224 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/mms/mmsEvent.py
--rw-r--r--   0        0        0     1327 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/mms/mmsImageEvent.py
--rw-r--r--   0        0        0     1327 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/mms/mmsVCardEvent.py
--rw-r--r--   0        0        0     1327 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/mms/mmsVideoEvent.py
--rw-r--r--   0        0        0      417 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/sms/ISMSEvent.py
--rw-r--r--   0        0        0      209 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/sms/ISMSMetadata.py
--rw-r--r--   0        0        0      200 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/sms/ISMSUsage.py
--rw-r--r--   0        0        0        0 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/sms/__init__.py
--rw-r--r--   0        0        0     1385 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/sms/smsEvent.py
--rw-r--r--   0        0        0     1168 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/sms/smsMetadata.py
--rw-r--r--   0        0        0     1150 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/sms/smsUsage.py
--rw-r--r--   0        0        0     1134 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/urlPayload.py
--rw-r--r--   0        0        0      270 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/viber/IViberEvent.py
--rw-r--r--   0        0        0        0 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/viber/__init__.py
--rw-r--r--   0        0        0     1248 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/viber/viberEvent.py
--rw-r--r--   0        0        0      328 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/webhookEventTypes.py
--rw-r--r--   0        0        0      222 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/whatsapp/IMessageEventContext.py
--rw-r--r--   0        0        0      185 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/whatsapp/IProfileName.py
--rw-r--r--   0        0        0      217 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/whatsapp/IReplyObject.py
--rw-r--r--   0        0        0      347 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/whatsapp/IWhatsappAudioEvent.py
--rw-r--r--   0        0        0      501 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/whatsapp/IWhatsappEvent.py
--rw-r--r--   0        0        0      345 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/whatsapp/IWhatsappFileEvent.py
--rw-r--r--   0        0        0      347 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/whatsapp/IWhatsappImageEvent.py
--rw-r--r--   0        0        0      359 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/whatsapp/IWhatsappReplyEvent.py
--rw-r--r--   0        0        0      277 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/whatsapp/IWhatsappTextEvent.py
--rw-r--r--   0        0        0      280 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/whatsapp/IWhatsappUnsupportedEvent.py
--rw-r--r--   0        0        0      347 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/whatsapp/IWhatsappVideoEvent.py
--rw-r--r--   0        0        0        0 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/whatsapp/__init__.py
--rw-r--r--   0        0        0     1210 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/whatsapp/messageEventContext.py
--rw-r--r--   0        0        0     1148 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/whatsapp/profileName.py
--rw-r--r--   0        0        0     1189 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/whatsapp/replyObject.py
--rw-r--r--   0        0        0     1617 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/whatsapp/whatsappAudioEvent.py
--rw-r--r--   0        0        0     1612 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/whatsapp/whatsappFileEvent.py
--rw-r--r--   0        0        0     1617 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/whatsapp/whatsappImageEvent.py
--rw-r--r--   0        0        0     1629 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/whatsapp/whatsappReplyEvent.py
--rw-r--r--   0        0        0     1544 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/whatsapp/whatsappTextEvent.py
--rw-r--r--   0        0        0     1558 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/whatsapp/whatsappUnsupportedEvent.py
--rw-r--r--   0        0        0     1617 2023-04-05 11:48:05.944852 nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/whatsapp/whatsappVideoEvent.py
--rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 nerualpha-4.1.0rc4/PKG-INFO
+-rw-r--r--   0        0        0      594 2023-04-11 15:54:47.931455 nerualpha-4.1.0rc5/README.md
+-rw-r--r--   0        0        0      843 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/pyproject.toml
+-rw-r--r--   0        0        0     1708 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/IBridge.py
+-rw-r--r--   0        0        0      853 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/INeru.py
+-rw-r--r--   0        0        0        0 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/__init__.py
+-rw-r--r--   0        0        0     4323 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/bridge.py
+-rw-r--r--   0        0        0     3926 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/neru.py
+-rw-r--r--   0        0        0        0 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/__init__.py
+-rw-r--r--   0        0        0     1356 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/assets/IAssets.py
+-rw-r--r--   0        0        0        0 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/assets/__init__.py
+-rw-r--r--   0        0        0     5963 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/assets/assets.py
+-rw-r--r--   0        0        0      316 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/assets/assetsActions.py
+-rw-r--r--   0        0        0        0 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/assets/contracts/__init__.py
+-rw-r--r--   0        0        0     1112 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/assets/contracts/assetInfo.py
+-rw-r--r--   0        0        0     1083 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/assets/contracts/assetLinkResponse.py
+-rw-r--r--   0        0        0     1149 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/assets/contracts/assetListResponse.py
+-rw-r--r--   0        0        0     1100 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/assets/contracts/directoryPayload.py
+-rw-r--r--   0        0        0     1087 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/assets/contracts/getAssetPayload.py
+-rw-r--r--   0        0        0     1098 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/assets/contracts/getAssetResponse.py
+-rw-r--r--   0        0        0     1145 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/assets/contracts/linkPayload.py
+-rw-r--r--   0        0        0     1212 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/assets/contracts/listAssetsPayload.py
+-rw-r--r--   0        0        0     1165 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/assets/contracts/removeAssetPayload.py
+-rw-r--r--   0        0        0      334 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/assets/fileRetentionPeriod.py
+-rw-r--r--   0        0        0      304 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/events/IEventEmitter.py
+-rw-r--r--   0        0        0      312 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/events/IEventFactory.py
+-rw-r--r--   0        0        0      388 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/events/INeruEvent.py
+-rw-r--r--   0        0        0      200 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/events/ISessionCreatedDetails.py
+-rw-r--r--   0        0        0        0 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/events/__init__.py
+-rw-r--r--   0        0        0     2804 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/events/eventEmitter.py
+-rw-r--r--   0        0        0     2389 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/events/eventFactory.py
+-rw-r--r--   0        0        0     1348 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/events/neruEvent.py
+-rw-r--r--   0        0        0      189 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/events/neruEventSourceTypes.py
+-rw-r--r--   0        0        0      477 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/events/neruEventTypes.py
+-rw-r--r--   0        0        0     1224 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/events/sessionCreatedDetails.py
+-rw-r--r--   0        0        0      447 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/logger/ILogAction.py
+-rw-r--r--   0        0        0      221 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/logger/ILogContext.py
+-rw-r--r--   0        0        0      311 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/logger/ILogger.py
+-rw-r--r--   0        0        0        0 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/logger/__init__.py
+-rw-r--r--   0        0        0     1415 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/logger/logAction.py
+-rw-r--r--   0        0        0     1292 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/logger/logContext.py
+-rw-r--r--   0        0        0      228 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/logger/logLevels.py
+-rw-r--r--   0        0        0     2990 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/logger/logger.py
+-rw-r--r--   0        0        0      212 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/logger/sourceTypes.py
+-rw-r--r--   0        0        0        0 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/__init__.py
+-rw-r--r--   0        0        0      199 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/ICreateRoomPayload.py
+-rw-r--r--   0        0        0        0 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/__init__.py
+-rw-r--r--   0        0        0     1667 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/createRoomPayload.py
+-rw-r--r--   0        0        0     1055 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/deleteRoomPayload.py
+-rw-r--r--   0        0        0     1274 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/getRoomsResponse.py
+-rw-r--r--   0        0        0     1194 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/pageLinks.py
+-rw-r--r--   0        0        0     1111 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/recordingOptions.py
+-rw-r--r--   0        0        0     1158 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/roomLinks.py
+-rw-r--r--   0        0        0     1465 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/roomResponse.py
+-rw-r--r--   0        0        0     1158 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/roomsEmbedded.py
+-rw-r--r--   0        0        0     1208 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/updateRoomDetails.py
+-rw-r--r--   0        0        0     1232 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/updateRoomPayload.py
+-rw-r--r--   0        0        0     3288 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/meetings.py
+-rw-r--r--   0        0        0      203 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/roomTypes.py
+-rw-r--r--   0        0        0     1596 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/IMessages.py
+-rw-r--r--   0        0        0        0 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/__init__.py
+-rw-r--r--   0        0        0      234 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IBaseMessage.py
+-rw-r--r--   0        0        0      198 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IImageData.py
+-rw-r--r--   0        0        0      495 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IListenEventsPayload.py
+-rw-r--r--   0        0        0      497 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IListenMessagesPayload.py
+-rw-r--r--   0        0        0      359 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IMMSAudioMessage.py
+-rw-r--r--   0        0        0      359 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IMMSImageMessage.py
+-rw-r--r--   0        0        0      359 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IMMSVCardMessage.py
+-rw-r--r--   0        0        0      359 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IMMSVideoMessage.py
+-rw-r--r--   0        0        0      215 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IMessageContact.py
+-rw-r--r--   0        0        0      199 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IMessenger.py
+-rw-r--r--   0        0        0      365 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IMessengerAudioMessage.py
+-rw-r--r--   0        0        0      363 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IMessengerFileMessage.py
+-rw-r--r--   0        0        0      365 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IMessengerImageMessage.py
+-rw-r--r--   0        0        0      194 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IMessengerTextMessage.py
+-rw-r--r--   0        0        0      365 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IMessengerVideoMessage.py
+-rw-r--r--   0        0        0      270 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/ISMSMessage.py
+-rw-r--r--   0        0        0      285 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/ISendImageContent.py
+-rw-r--r--   0        0        0      294 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/ISendImageMessage.py
+-rw-r--r--   0        0        0      426 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/ISendImagePayload.py
+-rw-r--r--   0        0        0      276 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/ISendImageResponse.py
+-rw-r--r--   0        0        0      194 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/ISendResponse.py
+-rw-r--r--   0        0        0      203 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/ISendTextContent.py
+-rw-r--r--   0        0        0      297 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/ISendTextMessagePayload.py
+-rw-r--r--   0        0        0      443 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/ISendTextPayload.py
+-rw-r--r--   0        0        0      199 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IURLPayload.py
+-rw-r--r--   0        0        0      196 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IUnsubscribeEventsPayload.py
+-rw-r--r--   0        0        0      361 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IViberImageMessage.py
+-rw-r--r--   0        0        0      216 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IViberService.py
+-rw-r--r--   0        0        0      276 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IViberTextMessage.py
+-rw-r--r--   0        0        0      199 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IWhatsapp.py
+-rw-r--r--   0        0        0      364 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IWhatsappAudioMessage.py
+-rw-r--r--   0        0        0      362 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IWhatsappFileMessage.py
+-rw-r--r--   0        0        0      364 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IWhatsappImageMessage.py
+-rw-r--r--   0        0        0      215 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IWhatsappTemplate.py
+-rw-r--r--   0        0        0      482 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IWhatsappTemplateMessage.py
+-rw-r--r--   0        0        0      279 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IWhatsappTextMessage.py
+-rw-r--r--   0        0        0      364 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IWhatsappVideoMessage.py
+-rw-r--r--   0        0        0        0 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/__init__.py
+-rw-r--r--   0        0        0     1206 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/baseMessage.py
+-rw-r--r--   0        0        0     1220 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/imageData.py
+-rw-r--r--   0        0        0     1492 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/listenEventsPayload.py
+-rw-r--r--   0        0        0     1500 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/listenMessagesPayload.py
+-rw-r--r--   0        0        0     1202 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/messageContact.py
+-rw-r--r--   0        0        0     1508 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/messengerAudioMessage.py
+-rw-r--r--   0        0        0     1502 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/messengerFileMessage.py
+-rw-r--r--   0        0        0     1508 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/messengerImageMessage.py
+-rw-r--r--   0        0        0     1419 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/messengerTextMessage.py
+-rw-r--r--   0        0        0     1508 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/messengerVideoMessage.py
+-rw-r--r--   0        0        0     1385 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/mmsAudioMessage.py
+-rw-r--r--   0        0        0     1372 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/mmsImageMessage.py
+-rw-r--r--   0        0        0     1372 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/mmsVCardMessage.py
+-rw-r--r--   0        0        0     1372 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/mmsVideoMessage.py
+-rw-r--r--   0        0        0     1330 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/sendImageContent.py
+-rw-r--r--   0        0        0     1309 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/sendImageMessage.py
+-rw-r--r--   0        0        0     1679 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/sendImagePayload.py
+-rw-r--r--   0        0        0     1166 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/sendResponse.py
+-rw-r--r--   0        0        0     1235 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/sendTextContent.py
+-rw-r--r--   0        0        0     1330 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/sendTextMessagePayload.py
+-rw-r--r--   0        0        0     1729 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/sendTextPayload.py
+-rw-r--r--   0        0        0     1267 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/smsMessage.py
+-rw-r--r--   0        0        0     1220 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/unsubscribeEventsPayload.py
+-rw-r--r--   0        0        0     1173 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/urlPayload.py
+-rw-r--r--   0        0        0     1509 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/viberImageMessage.py
+-rw-r--r--   0        0        0     1420 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/viberTextMessage.py
+-rw-r--r--   0        0        0     1397 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/whatsappAudioMessage.py
+-rw-r--r--   0        0        0     1391 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/whatsappFileMessage.py
+-rw-r--r--   0        0        0     1397 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/whatsappImageMessage.py
+-rw-r--r--   0        0        0     1528 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/whatsappTemplateMessage.py
+-rw-r--r--   0        0        0     1308 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/whatsappTextMessage.py
+-rw-r--r--   0        0        0     1397 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/whatsappVideoMessage.py
+-rw-r--r--   0        0        0      317 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/messageActions.py
+-rw-r--r--   0        0        0      219 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/messageChannelType.py
+-rw-r--r--   0        0        0      298 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/messageType.py
+-rw-r--r--   0        0        0     4786 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/messages.py
+-rw-r--r--   0        0        0        0 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/__init__.py
+-rw-r--r--   0        0        0      187 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/IBaseNumberOptions.py
+-rw-r--r--   0        0        0      411 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/IGetNumbersOptions.py
+-rw-r--r--   0        0        0      331 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/INumberOptions.py
+-rw-r--r--   0        0        0      403 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/ISearchNumbersOptions.py
+-rw-r--r--   0        0        0      450 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/IUpdateNumberOptions.py
+-rw-r--r--   0        0        0        0 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/__init__.py
+-rw-r--r--   0        0        0     1163 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/baseNumberOptions.py
+-rw-r--r--   0        0        0     1453 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/getNumbersOptions.py
+-rw-r--r--   0        0        0     1185 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/getNumbersResponse.py
+-rw-r--r--   0        0        0     1315 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/numberOptions.py
+-rw-r--r--   0        0        0     1259 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/numberResponse.py
+-rw-r--r--   0        0        0     1129 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/numbersOperationResponse.py
+-rw-r--r--   0        0        0     1515 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/searchNumbersOptions.py
+-rw-r--r--   0        0        0     1492 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/updateNumberOptions.py
+-rw-r--r--   0        0        0      208 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/numberFeature.py
+-rw-r--r--   0        0        0     7697 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/numbers.py
+-rw-r--r--   0        0        0     1672 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/queue/IQueue.py
+-rw-r--r--   0        0        0        0 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/queue/__init__.py
+-rw-r--r--   0        0        0      236 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/queue/contracts/ICreateQueueOptions.py
+-rw-r--r--   0        0        0      392 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/queue/contracts/ICreateQueuePayload.py
+-rw-r--r--   0        0        0      386 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/queue/contracts/IQueueDetails.py
+-rw-r--r--   0        0        0      280 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/queue/contracts/IQueueDetailsStats.py
+-rw-r--r--   0        0        0      211 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/queue/contracts/IQueueRate.py
+-rw-r--r--   0        0        0      220 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/queue/contracts/IUpdateQueueOptions.py
+-rw-r--r--   0        0        0      269 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/queue/contracts/IUpdateQueuePayload.py
+-rw-r--r--   0        0        0        0 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/queue/contracts/__init__.py
+-rw-r--r--   0        0        0     1225 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/queue/contracts/createQueueOptions.py
+-rw-r--r--   0        0        0     1382 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/queue/contracts/createQueuePayload.py
+-rw-r--r--   0        0        0      402 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/queue/contracts/queueDetailsResponse.py
+-rw-r--r--   0        0        0     1172 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/queue/contracts/queueRate.py
+-rw-r--r--   0        0        0     1208 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/queue/contracts/updateQueueOptions.py
+-rw-r--r--   0        0        0     1256 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/queue/contracts/updateQueuePayload.py
+-rw-r--r--   0        0        0     6959 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/queue/queue.py
+-rw-r--r--   0        0        0     1044 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/IScheduler.py
+-rw-r--r--   0        0        0        0 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/__init__.py
+-rw-r--r--   0        0        0      289 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/IIntervalParams.py
+-rw-r--r--   0        0        0      208 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/IListAllPayload.py
+-rw-r--r--   0        0        0      187 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/ISchedulePayload.py
+-rw-r--r--   0        0        0      374 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/IStartAtParams.py
+-rw-r--r--   0        0        0      447 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/IStartAtPayload.py
+-rw-r--r--   0        0        0      208 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/IUntilParams.py
+-rw-r--r--   0        0        0        0 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/__init__.py
+-rw-r--r--   0        0        0     1381 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/getSchedulerResponse.py
+-rw-r--r--   0        0        0     1269 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/intervalParams.py
+-rw-r--r--   0        0        0     1305 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/listAllPayload.py
+-rw-r--r--   0        0        0     1123 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/listAllSchedulersResponse.py
+-rw-r--r--   0        0        0     1138 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/schedulerExecutionInfo.py
+-rw-r--r--   0        0        0     1186 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/schedulerPayload.py
+-rw-r--r--   0        0        0     1375 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/startAtParams.py
+-rw-r--r--   0        0        0     1456 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/startAtPayload.py
+-rw-r--r--   0        0        0     1179 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/untilParams.py
+-rw-r--r--   0        0        0     3999 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/scheduler.py
+-rw-r--r--   0        0        0      237 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/schedulerActions.py
+-rw-r--r--   0        0        0     1971 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/state/IState.py
+-rw-r--r--   0        0        0      240 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/state/IStateCommand.py
+-rw-r--r--   0        0        0        0 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/state/__init__.py
+-rw-r--r--   0        0        0      212 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/state/expireOptions.py
+-rw-r--r--   0        0        0     9864 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/state/state.py
+-rw-r--r--   0        0        0     1341 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/state/stateCommand.py
+-rw-r--r--   0        0        0      694 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/state/stateOperations.py
+-rw-r--r--   0        0        0     4370 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/IConversation.py
+-rw-r--r--   0        0        0     1208 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/IUsers.py
+-rw-r--r--   0        0        0     1636 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/IVoice.py
+-rw-r--r--   0        0        0        0 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/__init__.py
+-rw-r--r--   0        0        0      207 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/callDirections.py
+-rw-r--r--   0        0        0      257 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/callStatuses.py
+-rw-r--r--   0        0        0      344 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IAcceptInboundCallBody.py
+-rw-r--r--   0        0        0      215 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IAcceptInboundCallEndpoint.py
+-rw-r--r--   0        0        0      403 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IAcceptInboundCallEvent.py
+-rw-r--r--   0        0        0      460 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IAcceptInboundCallPayload.py
+-rw-r--r--   0        0        0      209 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IAddUserPayload.py
+-rw-r--r--   0        0        0      225 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IAudioSettings.py
+-rw-r--r--   0        0        0      536 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IChannel.py
+-rw-r--r--   0        0        0      190 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IChannelEndpoint.py
+-rw-r--r--   0        0        0      291 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IChannelPhoneEndpoint.py
+-rw-r--r--   0        0        0      346 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IChannelSIPEndpoint.py
+-rw-r--r--   0        0        0      292 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IChannelVBCEndpoint.py
+-rw-r--r--   0        0        0      304 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IConversationPayloadWithCallback.py
+-rw-r--r--   0        0        0      220 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/ICreateConversationPayload.py
+-rw-r--r--   0        0        0      250 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/ICreateUserPayload.py
+-rw-r--r--   0        0        0      277 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IDeleteMemberPayload.py
+-rw-r--r--   0        0        0      214 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IEarmuffPayload.py
+-rw-r--r--   0        0        0      371 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IInviteMemberPayload.py
+-rw-r--r--   0        0        0      179 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/ILeg.py
+-rw-r--r--   0        0        0      293 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IMedia.py
+-rw-r--r--   0        0        0      211 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IMutePayload.py
+-rw-r--r--   0        0        0      423 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IOnInboundCallPayload.py
+-rw-r--r--   0        0        0      189 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IPlayStopBody.py
+-rw-r--r--   0        0        0      300 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IPlayStopPayload.py
+-rw-r--r--   0        0        0      241 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IPlayStreamBody.py
+-rw-r--r--   0        0        0      308 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IPlayStreamPayload.py
+-rw-r--r--   0        0        0      193 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IReason.py
+-rw-r--r--   0        0        0      187 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/ISayStopBody.py
+-rw-r--r--   0        0        0      296 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/ISayStopPayload.py
+-rw-r--r--   0        0        0      291 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/ISayTextBody.py
+-rw-r--r--   0        0        0      293 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/ISayTextParams.py
+-rw-r--r--   0        0        0      285 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/ISayTextPayload.py
+-rw-r--r--   0        0        0      373 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/ITransferMemberPayload.py
+-rw-r--r--   0        0        0      250 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IUpdateUserPayload.py
+-rw-r--r--   0        0        0      251 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IUser.py
+-rw-r--r--   0        0        0      277 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IVapiAnswerCallBack.py
+-rw-r--r--   0        0        0      274 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IVapiCreateCallOptions.py
+-rw-r--r--   0        0        0      373 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IVapiCreateCallPayload.py
+-rw-r--r--   0        0        0      312 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IVapiEventCallBackPayload.py
+-rw-r--r--   0        0        0      233 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IVapiEventParams.py
+-rw-r--r--   0        0        0     1063 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/Link.py
+-rw-r--r--   0        0        0        0 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/__init__.py
+-rw-r--r--   0        0        0     1341 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/acceptInboundCallBody.py
+-rw-r--r--   0        0        0     1224 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/acceptInboundCallEndpoint.py
+-rw-r--r--   0        0        0     1407 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/acceptInboundCallEvent.py
+-rw-r--r--   0        0        0     1824 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/acceptInboundCallPayload.py
+-rw-r--r--   0        0        0     1240 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/addUserPayload.py
+-rw-r--r--   0        0        0     1351 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/addUserResponse.py
+-rw-r--r--   0        0        0     1261 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/audioSayResponseBody.py
+-rw-r--r--   0        0        0     1078 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/audioSayStopResponseBody.py
+-rw-r--r--   0        0        0     1308 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/audioSettings.py
+-rw-r--r--   0        0        0     1605 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/channel.py
+-rw-r--r--   0        0        0     1315 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/channelAppEndpoint.py
+-rw-r--r--   0        0        0     1342 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/channelPhoneEndpoint.py
+-rw-r--r--   0        0        0     1626 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/channelSIPEndpoint.py
+-rw-r--r--   0        0        0     1344 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/channelVBCEndpoint.py
+-rw-r--r--   0        0        0     1430 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/conversationPayloadWithCallback.py
+-rw-r--r--   0        0        0     1133 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/conversationTimestamp.py
+-rw-r--r--   0        0        0     1303 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/createConversationPayload.py
+-rw-r--r--   0        0        0     1522 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/createConversationResponse.py
+-rw-r--r--   0        0        0     1428 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/createUserPayload.py
+-rw-r--r--   0        0        0     1399 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/deleteMemberPayload.py
+-rw-r--r--   0        0        0     1501 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/earmuffPayload.py
+-rw-r--r--   0        0        0     1073 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/earmuffResponseBody.py
+-rw-r--r--   0        0        0     1152 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/embeddedUsers.py
+-rw-r--r--   0        0        0     1229 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/eventEmbedded.py
+-rw-r--r--   0        0        0     1396 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/eventResponse.py
+-rw-r--r--   0        0        0     1271 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/getUsersResponse.py
+-rw-r--r--   0        0        0     1751 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/inviteMemberPayload.py
+-rw-r--r--   0        0        0     1121 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/leg.py
+-rw-r--r--   0        0        0     1315 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/media.py
+-rw-r--r--   0        0        0     1063 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/member.py
+-rw-r--r--   0        0        0     1570 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/memberResponse.py
+-rw-r--r--   0        0        0     1121 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/memberTimestamp.py
+-rw-r--r--   0        0        0     1483 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/mutePayload.py
+-rw-r--r--   0        0        0     1070 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/muteResponseBody.py
+-rw-r--r--   0        0        0     1571 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/onInboundCallPayload.py
+-rw-r--r--   0        0        0     1187 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/playStopBody.py
+-rw-r--r--   0        0        0     1572 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/playStopPayload.py
+-rw-r--r--   0        0        0     1226 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/playStreamBody.py
+-rw-r--r--   0        0        0     1490 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/playStreamPayload.py
+-rw-r--r--   0        0        0     1155 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/playStreamResponseBody.py
+-rw-r--r--   0        0        0     1081 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/playStreamStopResponseBody.py
+-rw-r--r--   0        0        0     1197 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/reason.py
+-rw-r--r--   0        0        0     1122 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/responseProperties.py
+-rw-r--r--   0        0        0     1179 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/sayStopBody.py
+-rw-r--r--   0        0        0     1559 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/sayStopPayload.py
+-rw-r--r--   0        0        0     1313 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/sayTextBody.py
+-rw-r--r--   0        0        0     1321 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/sayTextParams.py
+-rw-r--r--   0        0        0     1468 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/sayTextPayload.py
+-rw-r--r--   0        0        0     1126 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/selfLink.py
+-rw-r--r--   0        0        0     1966 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/transferMemberPayload.py
+-rw-r--r--   0        0        0     1456 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/updateUserPayload.py
+-rw-r--r--   0        0        0     1235 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/user.py
+-rw-r--r--   0        0        0     1123 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/userEmbedded.py
+-rw-r--r--   0        0        0     1453 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/userResponse.py
+-rw-r--r--   0        0        0     1184 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/userSummary.py
+-rw-r--r--   0        0        0     1125 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/userTimestamp.py
+-rw-r--r--   0        0        0     1294 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/vapiAnswerCallBack.py
+-rw-r--r--   0        0        0     1301 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/vapiCreateCallOptions.py
+-rw-r--r--   0        0        0     2231 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/vapiCreateCallPayload.py
+-rw-r--r--   0        0        0     1136 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/vapiCreateCallResponse.py
+-rw-r--r--   0        0        0     1338 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/vapiEventCallBackPayload.py
+-rw-r--r--   0        0        0     1227 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/vapiEventParams.py
+-rw-r--r--   0        0        0    11681 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/conversation.py
+-rw-r--r--   0        0        0      253 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/csChannelTypes.py
+-rw-r--r--   0        0        0      743 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/csEvents.py
+-rw-r--r--   0        0        0      174 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/memberActions.py
+-rw-r--r--   0        0        0      243 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/memberStates.py
+-rw-r--r--   0        0        0     3730 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/users.py
+-rw-r--r--   0        0        0     7104 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/voice.py
+-rw-r--r--   0        0        0      405 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/voiceActions.py
+-rw-r--r--   0        0        0      414 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAI/IVonageAI.py
+-rw-r--r--   0        0        0        0 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAI/__init__.py
+-rw-r--r--   0        0        0      193 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAI/contracts/IImportPayload.py
+-rw-r--r--   0        0        0      288 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAI/contracts/IVonageAiAnalyzePayload.py
+-rw-r--r--   0        0        0      384 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAI/contracts/IVonageAiImportModelPayload.py
+-rw-r--r--   0        0        0        0 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAI/contracts/__init__.py
+-rw-r--r--   0        0        0     1208 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAI/contracts/importPayload.py
+-rw-r--r--   0        0        0     1369 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAI/contracts/vonageAiAnalyzePayload.py
+-rw-r--r--   0        0        0     1489 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAI/contracts/vonageAiImportModelPayload.py
+-rw-r--r--   0        0        0     2513 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAI/vonageAI.py
+-rw-r--r--   0        0        0      209 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAI/vonageAIActions.py
+-rw-r--r--   0        0        0      385 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAPI/IVonageAPI.py
+-rw-r--r--   0        0        0        0 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAPI/__init__.py
+-rw-r--r--   0        0        0      241 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAPI/contracts/IInvokePayload.py
+-rw-r--r--   0        0        0        0 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAPI/contracts/__init__.py
+-rw-r--r--   0        0        0     1304 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAPI/contracts/invokePayload.py
+-rw-r--r--   0        0        0     1775 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAPI/vonageAPI.py
+-rw-r--r--   0        0        0      181 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAPI/vonageAPIActions.py
+-rw-r--r--   0        0        0      222 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/request/IFormDataObject.py
+-rw-r--r--   0        0        0      194 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/request/IRequest.py
+-rw-r--r--   0        0        0      356 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/request/IRequestParams.py
+-rw-r--r--   0        0        0        0 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/request/__init__.py
+-rw-r--r--   0        0        0     1181 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/request/formDataObject.py
+-rw-r--r--   0        0        0     1130 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/request/request.py
+-rw-r--r--   0        0        0      288 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/request/requestMethods.py
+-rw-r--r--   0        0        0     1335 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/request/requestParams.py
+-rw-r--r--   0        0        0      264 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/request/responseTypes.py
+-rw-r--r--   0        0        0        0 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/services/__init__.py
+-rw-r--r--   0        0        0      276 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/services/commandService/ICommandService.py
+-rw-r--r--   0        0        0        0 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/services/commandService/__init__.py
+-rw-r--r--   0        0        0     1697 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/services/commandService/commandService.py
+-rw-r--r--   0        0        0      551 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/services/config/IConfig.py
+-rw-r--r--   0        0        0      234 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/services/config/IPathObject.py
+-rw-r--r--   0        0        0        0 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/services/config/__init__.py
+-rw-r--r--   0        0        0     4016 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/services/config/config.py
+-rw-r--r--   0        0        0     1191 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/services/config/pathObject.py
+-rw-r--r--   0        0        0      201 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/services/jwt/IAcl.py
+-rw-r--r--   0        0        0      242 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/services/jwt/ICreateVonageTokenParams.py
+-rw-r--r--   0        0        0      437 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/services/jwt/IJwt.py
+-rw-r--r--   0        0        0        0 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/services/jwt/__init__.py
+-rw-r--r--   0        0        0     1130 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/services/jwt/acl.py
+-rw-r--r--   0        0        0     1247 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/services/jwt/createVonageTokenParams.py
+-rw-r--r--   0        0        0     3103 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/services/jwt/jwt.py
+-rw-r--r--   0        0        0     1224 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/services/jwt/neruJWTPayload.py
+-rw-r--r--   0        0        0     1203 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/services/jwt/vonageJWTPayload.py
+-rw-r--r--   0        0        0      405 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/session/IActionPayload.py
+-rw-r--r--   0        0        0      318 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/session/ICommand.py
+-rw-r--r--   0        0        0      212 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/session/IFilter.py
+-rw-r--r--   0        0        0      274 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/session/IPayloadWithCallback.py
+-rw-r--r--   0        0        0      281 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/session/IRequestInterface.py
+-rw-r--r--   0        0        0     1203 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/session/ISession.py
+-rw-r--r--   0        0        0      337 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/session/IWrappedCallback.py
+-rw-r--r--   0        0        0        0 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/session/__init__.py
+-rw-r--r--   0        0        0     1601 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/session/actionPayload.py
+-rw-r--r--   0        0        0     1324 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/session/command.py
+-rw-r--r--   0        0        0     1229 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/session/filter.py
+-rw-r--r--   0        0        0     5721 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/session/neruSession.py
+-rw-r--r--   0        0        0     1280 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/session/payloadWithCallback.py
+-rw-r--r--   0        0        0     1827 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/session/requestInterface.py
+-rw-r--r--   0        0        0     1665 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/session/requestInterfaceForCallbacks.py
+-rw-r--r--   0        0        0     1541 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/session/requestInterfaceWithParams.py
+-rw-r--r--   0        0        0     1302 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/session/wrappedCallback.py
+-rw-r--r--   0        0        0        0 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/smokes/__init__.py
+-rw-r--r--   0        0        0     2180 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/smokes/assetsTest.py
+-rw-r--r--   0        0        0     4230 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/smokes/messagesTest.py
+-rw-r--r--   0        0        0     3884 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/smokes/schedulerTest.py
+-rw-r--r--   0        0        0     1106 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/smokes/schedulerTestPayload.py
+-rw-r--r--   0        0        0     2734 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/smokes/stateTest.py
+-rw-r--r--   0        0        0     3983 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/smokes/voiceTest.py
+-rw-r--r--   0        0        0      250 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/IBaseEvent.py
+-rw-r--r--   0        0        0      183 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/IUrlPayload.py
+-rw-r--r--   0        0        0        0 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/__init__.py
+-rw-r--r--   0        0        0     1202 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/baseEvent.py
+-rw-r--r--   0        0        0      261 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/IMessangerEvent.py
+-rw-r--r--   0        0        0      352 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/IMessengerAudioEvent.py
+-rw-r--r--   0        0        0      350 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/IMessengerFileEvent.py
+-rw-r--r--   0        0        0      352 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/IMessengerImageEvent.py
+-rw-r--r--   0        0        0      282 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/IMessengerTextEvent.py
+-rw-r--r--   0        0        0      285 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/IMessengerUnsupportedEvent.py
+-rw-r--r--   0        0        0      352 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/IMessengerVideoEvent.py
+-rw-r--r--   0        0        0        0 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/__init__.py
+-rw-r--r--   0        0        0     1357 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/messengerAudioEvent.py
+-rw-r--r--   0        0        0     1254 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/messengerEvent.py
+-rw-r--r--   0        0        0     1352 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/messengerFileEvent.py
+-rw-r--r--   0        0        0     1357 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/messengerImageEvent.py
+-rw-r--r--   0        0        0     1284 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/messengerTextEvent.py
+-rw-r--r--   0        0        0     1298 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/messengerUnsupportedEvent.py
+-rw-r--r--   0        0        0     1357 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/messengerVideoEvent.py
+-rw-r--r--   0        0        0      322 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/mms/IMMSAudioEvent.py
+-rw-r--r--   0        0        0      255 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/mms/IMMSEvent.py
+-rw-r--r--   0        0        0      322 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/mms/IMMSImageEvent.py
+-rw-r--r--   0        0        0      322 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/mms/IMMSVCardEvent.py
+-rw-r--r--   0        0        0      322 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/mms/IMMSVideoEvent.py
+-rw-r--r--   0        0        0        0 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/mms/__init__.py
+-rw-r--r--   0        0        0     1327 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/mms/mmsAudioEvent.py
+-rw-r--r--   0        0        0     1224 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/mms/mmsEvent.py
+-rw-r--r--   0        0        0     1327 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/mms/mmsImageEvent.py
+-rw-r--r--   0        0        0     1327 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/mms/mmsVCardEvent.py
+-rw-r--r--   0        0        0     1327 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/mms/mmsVideoEvent.py
+-rw-r--r--   0        0        0      417 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/sms/ISMSEvent.py
+-rw-r--r--   0        0        0      209 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/sms/ISMSMetadata.py
+-rw-r--r--   0        0        0      200 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/sms/ISMSUsage.py
+-rw-r--r--   0        0        0        0 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/sms/__init__.py
+-rw-r--r--   0        0        0     1385 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/sms/smsEvent.py
+-rw-r--r--   0        0        0     1168 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/sms/smsMetadata.py
+-rw-r--r--   0        0        0     1150 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/sms/smsUsage.py
+-rw-r--r--   0        0        0     1134 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/urlPayload.py
+-rw-r--r--   0        0        0      270 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/viber/IViberEvent.py
+-rw-r--r--   0        0        0        0 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/viber/__init__.py
+-rw-r--r--   0        0        0     1248 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/viber/viberEvent.py
+-rw-r--r--   0        0        0      328 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/webhookEventTypes.py
+-rw-r--r--   0        0        0      222 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/IMessageEventContext.py
+-rw-r--r--   0        0        0      185 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/IProfileName.py
+-rw-r--r--   0        0        0      217 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/IReplyObject.py
+-rw-r--r--   0        0        0      347 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/IWhatsappAudioEvent.py
+-rw-r--r--   0        0        0      501 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/IWhatsappEvent.py
+-rw-r--r--   0        0        0      345 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/IWhatsappFileEvent.py
+-rw-r--r--   0        0        0      347 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/IWhatsappImageEvent.py
+-rw-r--r--   0        0        0      359 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/IWhatsappReplyEvent.py
+-rw-r--r--   0        0        0      277 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/IWhatsappTextEvent.py
+-rw-r--r--   0        0        0      280 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/IWhatsappUnsupportedEvent.py
+-rw-r--r--   0        0        0      347 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/IWhatsappVideoEvent.py
+-rw-r--r--   0        0        0        0 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/__init__.py
+-rw-r--r--   0        0        0     1210 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/messageEventContext.py
+-rw-r--r--   0        0        0     1148 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/profileName.py
+-rw-r--r--   0        0        0     1189 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/replyObject.py
+-rw-r--r--   0        0        0     1617 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/whatsappAudioEvent.py
+-rw-r--r--   0        0        0     1612 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/whatsappFileEvent.py
+-rw-r--r--   0        0        0     1617 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/whatsappImageEvent.py
+-rw-r--r--   0        0        0     1629 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/whatsappReplyEvent.py
+-rw-r--r--   0        0        0     1544 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/whatsappTextEvent.py
+-rw-r--r--   0        0        0     1558 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/whatsappUnsupportedEvent.py
+-rw-r--r--   0        0        0     1617 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/whatsappVideoEvent.py
+-rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 nerualpha-4.1.0rc5/PKG-INFO
```

### Comparing `nerualpha-4.1.0rc4/README.md` & `nerualpha-4.1.0rc5/README.md`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/pyproject.toml` & `nerualpha-4.1.0rc5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nerualpha"
-version = "4.1.0rc4"
+version = "4.1.0rc5"
 description = "neru-sdk for python developers"
 authors = ["Sergei Rastrigin <sergei.rastrigin@vonage.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10.5"
@@ -17,15 +17,15 @@
 bumpver = "^2022.1118"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.bumpver]
-current_version = "4.1.0rc4"
+current_version = "4.1.0rc5"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/IBridge.py` & `nerualpha-4.1.0rc5/src/nerualpha/IBridge.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/INeru.py` & `nerualpha-4.1.0rc5/src/nerualpha/INeru.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/bridge.py` & `nerualpha-4.1.0rc5/src/nerualpha/bridge.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/neru.py` & `nerualpha-4.1.0rc5/src/nerualpha/neru.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/assets/IAssets.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/assets/IAssets.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     @abstractmethod
     def getRemoteFile(self,remoteFilePath):
         pass
     @abstractmethod
     def generateLink(self,remoteFilePath,duration):
         pass
     @abstractmethod
-    def uploadFiles(self,localFilePaths,remoteDir):
+    def uploadFiles(self,localFilePaths,remoteDir,retentionPeriod = None):
         pass
     @abstractmethod
-    def uploadData(self,data,remoteDir,filenames = None):
+    def uploadData(self,data,remoteDir,filenames = None,retentionPeriod = None):
         pass
     @abstractmethod
     def list(self,remotePath,recursive,limit):
         pass
```

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/assets/assets.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/assets/assets.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from nerualpha.request.requestParams import RequestParams
 from nerualpha.providers.assets.contracts.linkPayload import LinkPayload
 from nerualpha.providers.assets.contracts.assetLinkResponse import AssetLinkResponse
 from nerualpha.providers.assets.contracts.assetListResponse import AssetListResponse
 from nerualpha.request.formDataObject import FormDataObject
 from nerualpha.request.IFormDataObject import IFormDataObject
 from nerualpha.request.responseTypes import ResponseTypes
+from nerualpha.providers.assets.fileRetentionPeriod import FileRetentionPeriod
 
 @dataclass
 class Assets(IAssets):
     bridge: IBridge
     session: ISession
     config: IConfig
     provider: str = field(default = "vonage-assets")
@@ -59,23 +60,23 @@
         requestParams = RequestParams()
         requestParams.method = RequestMethods.POST
         requestParams.data = LinkPayload(remoteFilePath,duration)
         requestParams.url = self.config.getExecutionUrl(self.provider,AssetsActions.Link)
         requestParams.headers = self.session.constructRequestHeaders()
         return RequestInterfaceWithParams(self.session,requestParams)
     
-    def uploadFiles(self,localFilePaths,remoteDir):
+    def uploadFiles(self,localFilePaths,remoteDir,retentionPeriod = None):
         streams = []
         for i in range(0,localFilePaths.__len__()):
             streams.append(self.bridge.createReadStream(localFilePaths[i]))
         
-        return self.uploadData(streams,remoteDir)
+        return self.uploadData(streams,remoteDir,None,retentionPeriod)
     
-    def uploadData(self,data,remoteDir,filenames = None):
-        url = self.config.getExecutionUrl(self.provider,AssetsActions.Copy,{"dst": remoteDir})
+    def uploadData(self,data,remoteDir,filenames = None,retentionPeriod = None):
+        url = self.config.getExecutionUrl(self.provider,AssetsActions.Copy,{"dst": remoteDir,"retention": retentionPeriod})
         requestParams = RequestParams()
         requestParams.method = RequestMethods.POST
         requestParams.data = []
         for i in range(0,data.__len__()):
             formData = FormDataObject()
             formData.name = f'file[{i}]'
             formData.value = data[i]
```

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/assets/contracts/assetInfo.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/assets/contracts/assetInfo.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/assets/contracts/assetLinkResponse.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/assets/contracts/assetLinkResponse.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/assets/contracts/assetListResponse.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/assets/contracts/assetListResponse.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/assets/contracts/directoryPayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/assets/contracts/directoryPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/assets/contracts/getAssetPayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/assets/contracts/getAssetPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/assets/contracts/getAssetResponse.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/assets/contracts/getAssetResponse.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/assets/contracts/linkPayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/assets/contracts/linkPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/assets/contracts/listAssetsPayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/assets/contracts/listAssetsPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/assets/contracts/removeAssetPayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/assets/contracts/removeAssetPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/events/eventEmitter.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/events/eventEmitter.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/events/eventFactory.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/events/eventFactory.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/events/neruEvent.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/events/neruEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/events/sessionCreatedDetails.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/events/sessionCreatedDetails.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/logger/logAction.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/logger/logAction.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/logger/logContext.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/logger/logContext.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/logger/logger.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/logger/logger.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/meetings/contracts/createRoomPayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/createRoomPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/meetings/contracts/deleteRoomPayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/deleteRoomPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/meetings/contracts/getRoomsResponse.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/getRoomsResponse.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/meetings/contracts/pageLinks.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/pageLinks.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/meetings/contracts/recordingOptions.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/recordingOptions.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/meetings/contracts/roomLinks.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/roomLinks.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/meetings/contracts/roomResponse.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/roomResponse.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/meetings/contracts/roomsEmbedded.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/roomsEmbedded.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/meetings/contracts/updateRoomDetails.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/updateRoomDetails.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/meetings/contracts/updateRoomPayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/updateRoomPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/meetings/meetings.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/meetings.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/messages/IMessages.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/IMessages.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/baseMessage.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/baseMessage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/imageData.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/imageData.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/listenEventsPayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/listenEventsPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/listenMessagesPayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/listenMessagesPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/messageContact.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/messageContact.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/messengerAudioMessage.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/messengerAudioMessage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/messengerFileMessage.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/messengerFileMessage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/messengerImageMessage.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/messengerImageMessage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/messengerTextMessage.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/messengerTextMessage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/messengerVideoMessage.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/messengerVideoMessage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/mmsAudioMessage.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/mmsAudioMessage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/mmsImageMessage.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/mmsImageMessage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/mmsVCardMessage.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/mmsVCardMessage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/mmsVideoMessage.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/mmsVideoMessage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/sendImageContent.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/sendImageContent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/sendImageMessage.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/sendImageMessage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/sendImagePayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/sendImagePayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/sendResponse.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/sendResponse.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/sendTextContent.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/sendTextContent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/sendTextMessagePayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/sendTextMessagePayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/sendTextPayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/sendTextPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/smsMessage.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/smsMessage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/unsubscribeEventsPayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/unsubscribeEventsPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/urlPayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/urlPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/viberImageMessage.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/viberImageMessage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/viberTextMessage.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/viberTextMessage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/whatsappAudioMessage.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/whatsappAudioMessage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/whatsappFileMessage.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/whatsappFileMessage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/whatsappImageMessage.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/whatsappImageMessage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/whatsappTemplateMessage.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/whatsappTemplateMessage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/whatsappTextMessage.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/whatsappTextMessage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/messages/contracts/whatsappVideoMessage.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/whatsappVideoMessage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/messages/messages.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/messages.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/numbers/contracts/baseNumberOptions.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/baseNumberOptions.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/numbers/contracts/getNumbersOptions.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/getNumbersOptions.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/numbers/contracts/getNumbersResponse.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/getNumbersResponse.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/numbers/contracts/numberOptions.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/numberOptions.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/numbers/contracts/numberResponse.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/numberResponse.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/numbers/contracts/numbersOperationResponse.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/numbersOperationResponse.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/numbers/contracts/searchNumbersOptions.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/searchNumbersOptions.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/numbers/contracts/updateNumberOptions.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/updateNumberOptions.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/numbers/numbers.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/numbers.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/queue/IQueue.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/queue/IQueue.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,7 +42,13 @@
         pass
     @abstractmethod
     def enqueue(self,name,data):
         pass
     @abstractmethod
     def enqueueSingle(self,name,data):
         pass
+    @abstractmethod
+    def deadLetterList(self,name):
+        pass
+    @abstractmethod
+    def deadLetterDequeue(self,name,count):
+        pass
```

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/queue/contracts/createQueueOptions.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/queue/contracts/createQueueOptions.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/queue/contracts/createQueuePayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/queue/contracts/createQueuePayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/queue/contracts/queueRate.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/queue/contracts/queueRate.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/queue/contracts/updateQueueOptions.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/queue/contracts/updateQueueOptions.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/queue/contracts/updateQueuePayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/queue/contracts/updateQueuePayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/queue/queue.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/queue/queue.py`

 * *Files 8% similar despite different names*

```diff
@@ -103,14 +103,30 @@
         requestParams.url = self.config.getExecutionUrl(self.provider,f'queue/{name}/enqueue')
         requestParams.headers = self.session.constructRequestHeaders()
         return RequestInterfaceWithParams(self.session,requestParams)
     
     def enqueueSingle(self,name,data):
         return self.enqueue(name,[data])
     
+    def deadLetterList(self,name):
+        requestParams = RequestParams()
+        requestParams.method = RequestMethods.GET
+        requestParams.data = None
+        requestParams.url = self.config.getExecutionUrl(self.provider,f'queue/{name}/deadletter')
+        requestParams.headers = self.session.constructRequestHeaders()
+        return RequestInterfaceWithParams(self.session,requestParams)
+    
+    def deadLetterDequeue(self,name,count = 1):
+        requestParams = RequestParams()
+        requestParams.method = RequestMethods.POST
+        requestParams.data = None
+        requestParams.url = self.config.getExecutionUrl(self.provider,f'queue/{name}/deadletter/pop',{"count": self.bridge.jsonStringify(count)})
+        requestParams.headers = self.session.constructRequestHeaders()
+        return RequestInterfaceWithParams(self.session,requestParams)
+    
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
         for key in dict:
             val = getattr(self, key)
```

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/scheduler/IScheduler.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/IScheduler.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/scheduler/contracts/getSchedulerResponse.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/getSchedulerResponse.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/scheduler/contracts/intervalParams.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/intervalParams.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/scheduler/contracts/listAllPayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/listAllPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/scheduler/contracts/listAllSchedulersResponse.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/listAllSchedulersResponse.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/scheduler/contracts/schedulerExecutionInfo.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/schedulerExecutionInfo.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/scheduler/contracts/schedulerPayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/schedulerPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/scheduler/contracts/startAtParams.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/startAtParams.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/scheduler/contracts/startAtPayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/startAtPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/scheduler/contracts/untilParams.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/untilParams.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/scheduler/scheduler.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/state/IState.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/state/IState.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/state/state.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/state/state.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/state/stateCommand.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/state/stateCommand.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/state/stateOperations.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/state/stateOperations.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/IConversation.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/IConversation.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/IUsers.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/IUsers.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/IVoice.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/IVoice.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/IChannel.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IChannel.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/Link.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/Link.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/acceptInboundCallBody.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/acceptInboundCallBody.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/acceptInboundCallEndpoint.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/acceptInboundCallEndpoint.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/acceptInboundCallEvent.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/acceptInboundCallEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/acceptInboundCallPayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/acceptInboundCallPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/addUserPayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/addUserPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/addUserResponse.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/addUserResponse.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/audioSayResponseBody.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/audioSayResponseBody.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/audioSayStopResponseBody.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/audioSayStopResponseBody.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/audioSettings.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/audioSettings.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/channel.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/channel.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/channelAppEndpoint.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/channelAppEndpoint.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/channelPhoneEndpoint.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/channelPhoneEndpoint.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/channelSIPEndpoint.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/channelSIPEndpoint.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/channelVBCEndpoint.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/channelVBCEndpoint.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/conversationPayloadWithCallback.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/conversationPayloadWithCallback.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/conversationTimestamp.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/conversationTimestamp.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/createConversationPayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/createConversationPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/createConversationResponse.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/createConversationResponse.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/createUserPayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/createUserPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/deleteMemberPayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/deleteMemberPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/earmuffPayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/earmuffPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/earmuffResponseBody.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/earmuffResponseBody.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/embeddedUsers.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/embeddedUsers.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/eventEmbedded.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/eventEmbedded.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/eventResponse.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/eventResponse.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/getUsersResponse.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/getUsersResponse.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/inviteMemberPayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/inviteMemberPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/leg.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/leg.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/media.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/media.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/member.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/member.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/memberResponse.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/memberResponse.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/memberTimestamp.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/memberTimestamp.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/mutePayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/mutePayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/muteResponseBody.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/muteResponseBody.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/onInboundCallPayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/onInboundCallPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/playStopBody.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/playStopBody.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/playStopPayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/playStopPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/playStreamBody.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/playStreamBody.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/playStreamPayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/playStreamPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/playStreamResponseBody.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/playStreamResponseBody.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/playStreamStopResponseBody.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/playStreamStopResponseBody.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/reason.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/reason.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/responseProperties.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/responseProperties.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/sayStopBody.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/sayStopBody.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/sayStopPayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/sayStopPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/sayTextBody.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/sayTextBody.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/sayTextParams.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/sayTextParams.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/sayTextPayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/sayTextPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/selfLink.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/selfLink.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/transferMemberPayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/transferMemberPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/updateUserPayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/updateUserPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/user.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/user.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/userEmbedded.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/userEmbedded.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/userResponse.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/userResponse.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/userSummary.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/userSummary.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/userTimestamp.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/userTimestamp.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/vapiAnswerCallBack.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/vapiAnswerCallBack.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/vapiCreateCallOptions.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/vapiCreateCallOptions.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/vapiCreateCallPayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/vapiCreateCallPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/vapiCreateCallResponse.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/vapiCreateCallResponse.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/vapiEventCallBackPayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/vapiEventCallBackPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/contracts/vapiEventParams.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/vapiEventParams.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/conversation.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/conversation.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/csEvents.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/csEvents.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/users.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/users.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/voice/voice.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/voice.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/vonageAI/contracts/importPayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAI/contracts/importPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/vonageAI/contracts/vonageAiAnalyzePayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAI/contracts/vonageAiAnalyzePayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/vonageAI/contracts/vonageAiImportModelPayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAI/contracts/vonageAiImportModelPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/vonageAI/vonageAI.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAI/vonageAI.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/vonageAPI/contracts/invokePayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAPI/contracts/invokePayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/providers/vonageAPI/vonageAPI.py` & `nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAPI/vonageAPI.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/request/formDataObject.py` & `nerualpha-4.1.0rc5/src/nerualpha/request/formDataObject.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/request/request.py` & `nerualpha-4.1.0rc5/src/nerualpha/request/request.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/request/requestParams.py` & `nerualpha-4.1.0rc5/src/nerualpha/request/requestParams.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/services/commandService/commandService.py` & `nerualpha-4.1.0rc5/src/nerualpha/services/commandService/commandService.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/services/config/IConfig.py` & `nerualpha-4.1.0rc5/src/nerualpha/services/config/IConfig.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/services/config/config.py` & `nerualpha-4.1.0rc5/src/nerualpha/services/config/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,19 +69,22 @@
         
         return url
     
     def queryObjectToString(self,queryObject):
         keys = self.bridge.getObjectKeys(queryObject)
         queryString = ""
         for i in range(0,keys.__len__()):
-            key = self.bridge.encodeUriComponent(keys[i])
-            value = self.bridge.encodeUriComponent(queryObject[keys[i]])
-            queryString += f'{key}={value}'
-            if i < keys.__len__() - 1:
-                queryString += "&"
+            key = keys[i]
+            if queryObject[key] is not None:
+                encodedKey = self.bridge.encodeUriComponent(key)
+                value = self.bridge.encodeUriComponent(queryObject[key])
+                queryString += f'{encodedKey}={value}'
+                if i < keys.__len__() - 1:
+                    queryString += "&"
+                
             
         
         return queryString
     
     def reprJSON(self):
         result = {}
         dict = asdict(self)
```

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/services/config/pathObject.py` & `nerualpha-4.1.0rc5/src/nerualpha/services/config/pathObject.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/services/jwt/acl.py` & `nerualpha-4.1.0rc5/src/nerualpha/services/jwt/acl.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/services/jwt/createVonageTokenParams.py` & `nerualpha-4.1.0rc5/src/nerualpha/services/jwt/createVonageTokenParams.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/services/jwt/jwt.py` & `nerualpha-4.1.0rc5/src/nerualpha/services/jwt/jwt.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/services/jwt/neruJWTPayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/services/jwt/neruJWTPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/services/jwt/vonageJWTPayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/services/jwt/vonageJWTPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/session/ISession.py` & `nerualpha-4.1.0rc5/src/nerualpha/session/ISession.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/session/actionPayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/session/actionPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/session/command.py` & `nerualpha-4.1.0rc5/src/nerualpha/session/command.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/session/filter.py` & `nerualpha-4.1.0rc5/src/nerualpha/session/filter.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/session/neruSession.py` & `nerualpha-4.1.0rc5/src/nerualpha/session/neruSession.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/session/payloadWithCallback.py` & `nerualpha-4.1.0rc5/src/nerualpha/session/payloadWithCallback.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/session/requestInterface.py` & `nerualpha-4.1.0rc5/src/nerualpha/session/requestInterface.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/session/requestInterfaceForCallbacks.py` & `nerualpha-4.1.0rc5/src/nerualpha/session/requestInterfaceForCallbacks.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/session/requestInterfaceWithParams.py` & `nerualpha-4.1.0rc5/src/nerualpha/session/requestInterfaceWithParams.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/session/wrappedCallback.py` & `nerualpha-4.1.0rc5/src/nerualpha/session/wrappedCallback.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/smokes/assetsTest.py` & `nerualpha-4.1.0rc5/src/nerualpha/smokes/assetsTest.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/smokes/messagesTest.py` & `nerualpha-4.1.0rc5/src/nerualpha/smokes/messagesTest.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/smokes/schedulerTest.py` & `nerualpha-4.1.0rc5/src/nerualpha/smokes/schedulerTest.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/smokes/schedulerTestPayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/smokes/schedulerTestPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/smokes/stateTest.py` & `nerualpha-4.1.0rc5/src/nerualpha/smokes/stateTest.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/smokes/voiceTest.py` & `nerualpha-4.1.0rc5/src/nerualpha/smokes/voiceTest.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/baseEvent.py` & `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/baseEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/messenger/messengerAudioEvent.py` & `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/messengerAudioEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/messenger/messengerEvent.py` & `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/messengerEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/messenger/messengerFileEvent.py` & `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/messengerFileEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/messenger/messengerImageEvent.py` & `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/messengerImageEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/messenger/messengerTextEvent.py` & `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/messengerTextEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/messenger/messengerUnsupportedEvent.py` & `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/messengerUnsupportedEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/messenger/messengerVideoEvent.py` & `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/messengerVideoEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/mms/mmsAudioEvent.py` & `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/mms/mmsAudioEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/mms/mmsEvent.py` & `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/mms/mmsEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/mms/mmsImageEvent.py` & `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/mms/mmsImageEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/mms/mmsVCardEvent.py` & `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/mms/mmsVCardEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/mms/mmsVideoEvent.py` & `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/mms/mmsVideoEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/sms/smsEvent.py` & `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/sms/smsEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/sms/smsMetadata.py` & `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/sms/smsMetadata.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/sms/smsUsage.py` & `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/sms/smsUsage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/urlPayload.py` & `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/urlPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/viber/viberEvent.py` & `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/viber/viberEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/whatsapp/messageEventContext.py` & `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/messageEventContext.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/whatsapp/profileName.py` & `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/profileName.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/whatsapp/replyObject.py` & `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/replyObject.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/whatsapp/whatsappAudioEvent.py` & `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/whatsappAudioEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/whatsapp/whatsappFileEvent.py` & `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/whatsappFileEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/whatsapp/whatsappImageEvent.py` & `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/whatsappImageEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/whatsapp/whatsappReplyEvent.py` & `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/whatsappReplyEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/whatsapp/whatsappTextEvent.py` & `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/whatsappTextEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/whatsapp/whatsappUnsupportedEvent.py` & `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/whatsappUnsupportedEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/src/nerualpha/webhookEvents/whatsapp/whatsappVideoEvent.py` & `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/whatsappVideoEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc4/PKG-INFO` & `nerualpha-4.1.0rc5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nerualpha
-Version: 4.1.0rc4
+Version: 4.1.0rc5
 Summary: neru-sdk for python developers
 License: MIT
 Author: Sergei Rastrigin
 Author-email: sergei.rastrigin@vonage.com
 Requires-Python: >=3.10.5,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

