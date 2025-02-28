---
title: class MipConfiguration 
description: Documents the mipconfiguration::undefined class of the Microsoft Information Protection (MIP) SDK.
author: msmbaldwin
ms.service: information-protection
ms.topic: reference
ms.author: mbaldwin
ms.date: 11/15/2021
---

# class MipConfiguration 
Configuration used by MIP sdk during its creation and throughout its lifetime.
  
## Summary
 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
public MipConfiguration(const ApplicationInfo& appInfo, const std::string& path, LogLevel thresholdLogLevel, bool isOfflineOnly)  | _Not yet documented._
public const ApplicationInfo& GetApplicationInfo() const  |  Get the Description of host application.
public const std::string& GetPath() const  |  Get the File path for logs, caches, etc.
public const LogLevel& GetThresholdLogLevel() const  |  Get the Minimum log level for .miplog.
public const bool isOfflineOnly() const  |  whether Network operations is enabled or disabled(not all actions supported when offline)
public std::shared_ptr\<DiagnosticConfiguration\> GetDiagnosticConfiguration() const  |  Get the Diagnostic (if any) provided by the application.
public void SetDiagnosticConfiguration(const std::shared_ptr\<DiagnosticConfiguration\>& diagnosticConfiguration)  |  Override default configuration of diagnostic.
public std::shared_ptr\<LoggerDelegate\> GetLoggerDelegate() const  |  Get the LoggerDelegate (if any) override implementation.
public void SetLoggerDelegate(const std::shared_ptr\<LoggerDelegate\>& loggerDelegate)  |  Set the LoggerDelegate (if any) override implementation.
public std::shared_ptr\<StorageDelegate\> GetStorageDelegate() const  |  Get the StorageDelegate (if any) override implementation.
public void SetStorageDelegate(const std::shared_ptr\<StorageDelegate\>& storageDelegate)  |  Set the StorageDelegate (if any) override implementation. It's a required delegate for MIP Core Context.
public std::shared_ptr\<HttpDelegate\> GetHttpDelegate() const  |  Get the HttpDelegate (if any) override implementation.
public void SetHttpDelegate(const std::shared_ptr\<HttpDelegate\>& httpDelegate)  |  Set the HttpDelegate (if any) override implementation. It's a required delegate for MIP Core Context.
public std::shared_ptr\<JsonDelegate\> GetJsonDelegate() const  |  Get the JsonDelegate (if any) override implementation.
public std::shared_ptr\<xml::XmlDelegate\> GetXmlDelegate() const  |  Get the XmlDelegate (if any) override implementation. MipConfiguration needs to be derived from to override the internal xmlDelegate with an alternative. This delegate is only configurable when using the MIP Core Context and only for the protection and upe sdk.
public std::map\<FlightingFeature, bool\> GetFeatureSettings() const  |  Get the Flighting features which should be set to non-default values.
public void SetFeatureSettings(const std::map\<FlightingFeature, bool\>& featureSettings)  |  Set the Flighting features which should be set to non-default values.
public ~MipConfiguration()  | _Not yet documented._
protected std::shared_ptr\<JsonDelegate\> mJsonDelegate  | _Not yet documented._
protected std::shared_ptr\<xml::XmlDelegate\> mXmlDelegate  | _Not yet documented._
  
## Members
  
### MipConfiguration function
_Not documented yet._

  
### GetApplicationInfo function
Get the Description of host application.

  
**Returns**: Description of host application
  
### GetPath function
Get the File path for logs, caches, etc.

  
**Returns**: File path for logs, caches, etc.
  
### GetThresholdLogLevel function
Get the Minimum log level for .miplog.

  
**Returns**: Minimum log level for .miplog.
  
### isOfflineOnly function
whether Network operations is enabled or disabled(not all actions supported when offline)

  
**Returns**: Network operations state
  
### GetDiagnosticConfiguration function
Get the Diagnostic (if any) provided by the application.

  
**Returns**: Diagnostic Configuration to be used for configuring telemetry/audit.
  
### SetDiagnosticConfiguration function
Override default configuration of diagnostic.

Parameters:  
* **diagnosticConfiguration**: diagnostic configuration to be used for configuring telemetry/audit.


  
### GetLoggerDelegate function
Get the LoggerDelegate (if any) override implementation.

  
**Returns**: LoggerDelegate (if any) override implementation.
  
### SetLoggerDelegate function
Set the LoggerDelegate (if any) override implementation.

Parameters:  
* **loggerDelegate**: LoggerDelegate override implementation


  
### GetStorageDelegate function
Get the StorageDelegate (if any) override implementation.

  
**Returns**: StorageDelegate (if any) override implementation.
  
### SetStorageDelegate function
Set the StorageDelegate (if any) override implementation. It's a required delegate for MIP Core Context.

Parameters:  
* **storageDelegate**: StorageDelegate override implementation


  
### GetHttpDelegate function
Get the HttpDelegate (if any) override implementation.

  
**Returns**: HttpDelegate (if any) override implementation.
  
### SetHttpDelegate function
Set the HttpDelegate (if any) override implementation. It's a required delegate for MIP Core Context.

Parameters:  
* **httpDelegate**: HttpDelegate override implementation


  
### GetJsonDelegate function
Get the JsonDelegate (if any) override implementation.

  
**Returns**: JsonDelegate (if any) override implementation.
  
### GetXmlDelegate function
Get the XmlDelegate (if any) override implementation. MipConfiguration needs to be derived from to override the internal xmlDelegate with an alternative. This delegate is only configurable when using the MIP Core Context and only for the protection and upe sdk.

  
**Returns**: XmlDelegate (if any) override implementation. nullptr by default.
  
### GetFeatureSettings function
Get the Flighting features which should be set to non-default values.

  
**Returns**: Flighting features which should be set to non-default values
  
### SetFeatureSettings function
Set the Flighting features which should be set to non-default values.

Parameters:  
* **featureSettings**: Flighting features to be used.


  
### ~MipConfiguration function
_Not documented yet._

  
### JsonDelegate
_Not documented yet._

  
### xml::XmlDelegate
_Not documented yet._
_
