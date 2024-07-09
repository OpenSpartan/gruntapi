<div align="center">
	<br>
	<br>
	<div>
		<picture>
			<img alt="GruntAPI logo" width="200px" src="media/logo.png">
		</picture>
		<br>
	</div>
	<h1>GruntAPI</h1>
	<p>
		An open-source Command Line Interface (CLI) for Halo Infinite data, powered by <a href="https://openspartan.com">OpenSpartan</a> tooling.
	</p>
	<br>
</div>

## Overview

GruntAPI is a cross-platform CLI that allows anyone who plays Halo Infinite to query their Halo Infinite data, such as match stats, inventory, battle pass progress, and more.

[📕 **Learn More - Official Documentation**](https://gruntapi.com)

## Getting started

Before you can query the data, you need to log in:

```bash
gruntapi login
```

You will be prompted to enter your Microsoft account credentials. Once you authenticate, you can run a range of commands to test that you're logged into the right account, such as:

```bash
gruntapi servicerecord
```

This should return the current player's service record. If the call is successful, you are authenticated.

## Commands

For a full list of commands and capabilities of GruntAPI, refer to the [official documentation](https://gruntapi.com).

### Get service record

```bash
gruntapi servicerecord
```

To get another player's service record:

```bash
gruntapi servicerecord --player-id GAMERTAG_OR_XUID
```

In the example above, `--player-id` can be either a player gamertag or their Xbox User ID (XUID) in the format `xuid(PLAYER_XUID)`.

### Get match history

```bash
gruntapi matchhistory
```

### Get specific match stats

```bash
gruntapi match --match-id MATCH_ID
```

### Get current inventory

```bash
gruntapi inventory
```

### Get season calendar

```bash
gruntapi seasoncalendar
```

### Get store offerings

```bash
gruntapi store --type generic
```

### Get HCS store offerings

```bash
gruntapi store --type hcs
```

### Get items on The Exchange

```bash
gruntapi store --type exchange
```

## Origins

GruntAPI [started](https://web.archive.org/web/20220907215813/https://gruntapi.com/) as a .NET-based wrapper for Halo Infinite. Since then, the library was made private, however the name got transferred to this project, providing Halo Infinite enthusiasts an avenue to query their game data from their favorite terminal application.
