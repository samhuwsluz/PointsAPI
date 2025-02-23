# Installation (Maven):
## Step1:
Add the JitPack repository to your build file:
```xml
<repository>
  <id>jitpack.io</id>
  <url>https://jitpack.io</url>
</repository>
```

## Step2:
Add the dependency
```xml
<dependency>
  <groupId>com.github.Samhuwsluz</groupId>
  <artifactId>PointsAPI</artifactId>
  <version>v0.0.1</version>
</dependency>
```

# API Usage
## Importing the API

```java
import ch.ksrminecraft.RangAPI.RangAPI
```

## Loading Plugin instance

```java
 import ch.ksrminecraft.RangAPI.RangAPI;

// Credentials to the Points DB
RangAPI api = new RangAPI(String url, String user, String pass);
```


# API Reference

## Get Points from User
```java
public int getPoints(UUID uuid);
```

## Set Points from User
```java
public void setPoints(UUID uuid, int points);
```

## Add Points to User
```java
public void addPoints(UUID uuid, int delta);
```

# Configuration (Plugin)
## DB-Schema
The Database should have a **Table** called **points**
This Table must have the Fields: **UUID:text, points:int(11), time:timestamp**
