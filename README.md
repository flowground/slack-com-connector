# ![LOGO](logo.png) Slack **flow**ground Connector

## Description

A generated **flow**ground connector for the Slack API (version 1.0.6).

Generated from: https://api.apis.guru/v2/specs/slack.com/1.0.6/swagger.json<br/>
Generated at: 2019-05-07T17:44:04+03:00

## API Description

One way to interact with the Slack platform is its HTTP RPC-based Web API, a collection of methods requiring OAuth 2.0-based user, bot, or workspace tokens blessed with related OAuth scopes.

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Checks API calling code.

*Tags:* `api`

#### Input Parameters
* `foo` - _optional_ - example property to return
* `error` - _optional_ - Error response to return

### Returns list of permissions this app has on a team.

*Tags:* `apps.permissions` `apps`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `none`

### Allows an app to request additional scopes

*Tags:* `apps.permissions` `apps`

#### Input Parameters
* `scopes` - _optional_ - A comma separated list of scopes to request for
* `token` - _optional_ - Authentication token. Requires scope: `none`
* `trigger_id` - _optional_ - Token used to trigger the permissions API

### Returns list of resource grants this app has on a team.

*Tags:* `apps.permissions.resources` `apps`

#### Input Parameters
* `cursor` - _optional_ - Paginate through collections of data by setting the `cursor` parameter to a `next_cursor` attribute returned by a previous request's `response_metadata`. Default value fetches the first "page" of the collection. See [pagination](/docs/pagination) for more detail.
* `token` - _optional_ - Authentication token. Requires scope: `none`
* `limit` - _optional_ - The maximum number of items to return.

### Returns list of scopes this app has on a team.

*Tags:* `apps.permissions.scopes` `apps`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `none`

### Revokes a token.

*Tags:* `auth`

#### Input Parameters
* `test` - _optional_ - Setting this parameter to `1` triggers a _testing mode_ where the specified token will not actually be revoked.
* `token` - _optional_ - Authentication token. Requires scope: `none`

### Checks authentication & identity.

*Tags:* `auth`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `none`

### Gets information about a bot user.

*Tags:* `bots`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `users:read`
* `bot` - _optional_ - Bot user to get info on

### Archives a channel.

*Tags:* `channels`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `channels:write`

### Creates a channel.

*Tags:* `channels`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `channels:write`

### Fetches history of messages and events from a channel.

*Tags:* `channels`

#### Input Parameters
* `count` - _optional_ - Number of messages to return, between 1 and 1000.
* `unreads` - _optional_ - Include `unread_count_display` in the output?
* `inclusive` - _optional_ - Include messages with latest or oldest timestamp in results.
* `token` - _optional_ - Authentication token. Requires scope: `channels:history`
* `oldest` - _optional_ - Start of time range of messages to include in results.
* `channel` - _optional_ - Channel to fetch history for.
* `latest` - _optional_ - End of time range of messages to include in results.

### Gets information about a channel.

*Tags:* `channels`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `channels:read`
* `include_locale` - _optional_ - Set this to `true` to receive the locale for this channel. Defaults to `false`
* `channel` - _optional_ - Channel to get info on

### Invites a user to a channel.

*Tags:* `channels`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `channels:write`

### Joins a channel, creating it if needed.

*Tags:* `channels`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `channels:write`

### Removes a user from a channel.

*Tags:* `channels`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `channels:write`

### Leaves a channel.

*Tags:* `channels`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `channels:write`

### Lists all channels in a Slack team.

*Tags:* `channels`

#### Input Parameters
* `exclude_members` - _optional_ - Exclude the `members` collection from each `channel`
* `cursor` - _optional_ - Paginate through collections of data by setting the `cursor` parameter to a `next_cursor` attribute returned by a previous request's `response_metadata`. Default value fetches the first "page" of the collection. See [pagination](/docs/pagination) for more detail.
* `token` - _optional_ - Authentication token. Requires scope: `channels:read`
* `limit` - _optional_ - The maximum number of items to return. Fewer than the requested number of items may be returned, even if the end of the users list hasn't been reached.
* `exclude_archived` - _optional_ - Exclude archived channels from the list

### Sets the read cursor in a channel.

*Tags:* `channels`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `channels:write`

### Renames a channel.

*Tags:* `channels`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `channels:write`

### Retrieve a thread of messages posted to a channel

*Tags:* `channels`

#### Input Parameters
* `thread_ts` - _optional_ - Unique identifier of a thread's parent message
* `token` - _optional_ - Authentication token. Requires scope: `channels:history`
* `channel` - _optional_ - Channel to fetch thread from

### Sets the purpose for a channel.

*Tags:* `channels`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `channels:write`

### Sets the topic for a channel.

*Tags:* `channels`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `channels:write`

### Unarchives a channel.

*Tags:* `channels`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `channels:write`

### Deletes a message.

*Tags:* `chat`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `chat:write`

### Retrieve a permalink URL for a specific extant message

*Tags:* `chat`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `none`
* `message_ts` - _optional_ - A message's `ts` value, uniquely identifying it within a channel
* `channel` - _optional_ - The ID of the conversation or channel containing the message

### Share a me message into a channel.

*Tags:* `chat`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `chat:write:user`

### Sends an ephemeral message to a user in a channel.

*Tags:* `chat`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `chat:write`

### Sends a message to a channel.

*Tags:* `chat`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `chat:write`

### Provide custom unfurl behavior for user-posted URLs

*Tags:* `chat`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `links:write`

### Updates a message.

*Tags:* `chat`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `chat:write`

### Archives a conversation.

*Tags:* `conversations`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `conversations:write`

### Closes a direct message or multi-person direct message.

*Tags:* `conversations`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `conversations:write`

### Initiates a public or private channel-based conversation

*Tags:* `conversations`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `conversations:write`

### Fetches a conversation's history of messages and events.

*Tags:* `conversations`

#### Input Parameters
* `inclusive` - _optional_ - Include messages with latest or oldest timestamp in results only when either timestamp is specified.
* `cursor` - _optional_ - Paginate through collections of data by setting the `cursor` parameter to a `next_cursor` attribute returned by a previous request's `response_metadata`. Default value fetches the first "page" of the collection. See [pagination](/docs/pagination) for more detail.
* `token` - _optional_ - Authentication token. Requires scope: `conversations:history`
* `limit` - _optional_ - The maximum number of items to return. Fewer than the requested number of items may be returned, even if the end of the users list hasn't been reached.
* `oldest` - _optional_ - Start of time range of messages to include in results.
* `channel` - _optional_ - Conversation ID to fetch history for.
* `latest` - _optional_ - End of time range of messages to include in results.

### Retrieve information about a conversation.

*Tags:* `conversations`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `conversations:read`
* `channel` - _optional_ - Conversation ID to learn more about
* `include_locale` - _optional_ - Set this to `true` to receive the locale for this conversation. Defaults to `false`

### Invites users to a channel.

*Tags:* `conversations`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `conversations:write`

### Joins an existing conversation.

*Tags:* `conversations`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `channels:write`

### Removes a user from a conversation.

*Tags:* `conversations`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `conversations:write`

### Leaves a conversation.

*Tags:* `conversations`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `conversations:write`

### Lists all channels in a Slack team.

*Tags:* `conversations`

#### Input Parameters
* `cursor` - _optional_ - Paginate through collections of data by setting the `cursor` parameter to a `next_cursor` attribute returned by a previous request's `response_metadata`. Default value fetches the first "page" of the collection. See [pagination](/docs/pagination) for more detail.
* `token` - _optional_ - Authentication token. Requires scope: `conversations:read`
* `limit` - _optional_ - The maximum number of items to return. Fewer than the requested number of items may be returned, even if the end of the list hasn't been reached. Must be an integer no larger than 1000.
* `exclude_archived` - _optional_ - Set to `true` to exclude archived channels from the list
* `types` - _optional_ - Mix and match channel types by providing a comma-separated list of any combination of `public_channel`, `private_channel`, `mpim`, `im`

### Retrieve members of a conversation.

*Tags:* `conversations`

#### Input Parameters
* `cursor` - _optional_ - Paginate through collections of data by setting the `cursor` parameter to a `next_cursor` attribute returned by a previous request's `response_metadata`. Default value fetches the first "page" of the collection. See [pagination](/docs/pagination) for more detail.
* `token` - _optional_ - Authentication token. Requires scope: `conversations:read`
* `limit` - _optional_ - The maximum number of items to return. Fewer than the requested number of items may be returned, even if the end of the users list hasn't been reached.
* `channel` - _optional_ - ID of the conversation to retrieve members for

### Opens or resumes a direct message or multi-person direct message.

*Tags:* `conversations`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `conversations:write`

### Renames a conversation.

*Tags:* `conversations`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `conversations:write`

### Retrieve a thread of messages posted to a conversation

*Tags:* `conversations`

#### Input Parameters
* `inclusive` - _optional_ - Include messages with latest or oldest timestamp in results only when either timestamp is specified.
* `ts` - _optional_ - Unique identifier of a thread's parent message.
* `cursor` - _optional_ - Paginate through collections of data by setting the `cursor` parameter to a `next_cursor` attribute returned by a previous request's `response_metadata`. Default value fetches the first "page" of the collection. See [pagination](/docs/pagination) for more detail.
* `token` - _optional_ - Authentication token. Requires scope: `conversations:history`
* `limit` - _optional_ - The maximum number of items to return. Fewer than the requested number of items may be returned, even if the end of the users list hasn't been reached.
* `oldest` - _optional_ - Start of time range of messages to include in results.
* `channel` - _optional_ - Conversation ID to fetch thread from.
* `latest` - _optional_ - End of time range of messages to include in results.

### Sets the purpose for a conversation.

*Tags:* `conversations`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `conversations:write`

### Sets the topic for a conversation.

*Tags:* `conversations`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `conversations:write`

### Reverses conversation archival.

*Tags:* `conversations`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `conversations:write`

### Open a dialog with a user

*Tags:* `dialog`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `none`
* `dialog` - _optional_ - The dialog definition. This must be a JSON-encoded string.
* `trigger_id` - _optional_ - Exchange a trigger to post to the user.

### Ends the current user's Do Not Disturb session immediately.

*Tags:* `dnd`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `dnd:write`

### Ends the current user's snooze mode immediately.

*Tags:* `dnd`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `dnd:write`

### Retrieves a user's current Do Not Disturb status.

*Tags:* `dnd`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `dnd:read`
* `user` - _optional_ - User to fetch status for (defaults to current user)

### Turns on Do Not Disturb mode for the current user, or changes its duration.

*Tags:* `dnd`

### Retrieves the Do Not Disturb status for users on a team.

*Tags:* `dnd`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `dnd:read`
* `users` - _optional_ - Comma-separated list of users to fetch Do Not Disturb status for

### Lists custom emoji for a team.

*Tags:* `emoji`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `emoji:read`

### Add a comment to an existing file.

*Tags:* `files.comments` `files`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `files:write:user`

### Deletes an existing comment on a file.

*Tags:* `files.comments` `files`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `files:write:user`

### Edit an existing file comment.

*Tags:* `files.comments` `files`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `files:write:user`

### Deletes a file.

*Tags:* `files`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `files:write:user`

### Gets information about a team file.

*Tags:* `files`

#### Input Parameters
* `count` - _optional_
* `token` - _optional_ - Authentication token. Requires scope: `files:read`
* `file` - _optional_ - Specify a file by providing its ID.
* `page` - _optional_

### Lists & filters team files.

*Tags:* `files`

#### Input Parameters
* `count` - _optional_
* `channel` - _optional_ - Filter files appearing in a specific channel, indicated by its ID.
* `ts_to` - _optional_ - Filter files created before this timestamp (inclusive).
* `ts_from` - _optional_ - Filter files created after this timestamp (inclusive).
* `token` - _optional_ - Authentication token. Requires scope: `files:read`
* `user` - _optional_ - Filter files created by a single user.
* `page` - _optional_
* `types` - _optional_ - Filter files by type:

* `all` - All files
* `spaces` - Posts
* `snippets` - Snippets
* `images` - Image files
* `gdocs` - Google docs
* `zips` - Zip files
* `pdfs` - PDF files

You can pass multiple values in the types argument, like `types=spaces,snippets`.The default value is `all`, which does not filter the list.

### Revokes public/external sharing access for a file

*Tags:* `files`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `files:write:user`

### Enables a file for public/external sharing.

*Tags:* `files`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `files:write:user`

### Uploads or creates a file.

*Tags:* `files`

### Archives a private channel.

*Tags:* `groups`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `groups:write`

### Creates a private channel.

*Tags:* `groups`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `groups:write`

### Clones and archives a private channel.

*Tags:* `groups`

### Fetches history of messages and events from a private channel.

*Tags:* `groups`

#### Input Parameters
* `count` - _optional_ - Number of messages to return, between 1 and 1000.
* `unreads` - _optional_ - Include `unread_count_display` in the output?
* `inclusive` - _optional_ - Include messages with latest or oldest timestamp in results.
* `token` - _optional_ - Authentication token. Requires scope: `groups:history`
* `oldest` - _optional_ - Start of time range of messages to include in results.
* `channel` - _optional_ - Private channel to fetch history for.
* `latest` - _optional_ - End of time range of messages to include in results.

### Gets information about a private channel.

*Tags:* `groups`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `groups:read`
* `include_locale` - _optional_ - Set this to `true` to receive the locale for this group. Defaults to `false`
* `channel` - _optional_ - Private channel to get info on

### Invites a user to a private channel.

*Tags:* `groups`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `groups:write`

### Removes a user from a private channel.

*Tags:* `groups`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `groups:write`

### Leaves a private channel.

*Tags:* `groups`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `groups:write`

### Lists private channels that the calling user has access to.

*Tags:* `groups`

#### Input Parameters
* `exclude_members` - _optional_ - Exclude the `members` from each `group`
* `token` - _optional_ - Authentication token. Requires scope: `groups:read`
* `exclude_archived` - _optional_ - Don't return archived private channels.

### Sets the read cursor in a private channel.

*Tags:* `groups`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `groups:write`

### Opens a private channel.

*Tags:* `groups`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `groups:write`

### Renames a private channel.

*Tags:* `groups`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `groups:write`

### Retrieve a thread of messages posted to a private channel

*Tags:* `groups`

#### Input Parameters
* `thread_ts` - _optional_ - Unique identifier of a thread's parent message
* `token` - _optional_ - Authentication token. Requires scope: `groups:history`
* `channel` - _optional_ - Private channel to fetch thread from

### Sets the purpose for a private channel.

*Tags:* `groups`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `groups:write`

### Sets the topic for a private channel.

*Tags:* `groups`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `groups:write`

### Unarchives a private channel.

*Tags:* `groups`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `groups:write`

### Close a direct message channel.

*Tags:* `im`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `im:write`

### Fetches history of messages and events from direct message channel.

*Tags:* `im`

#### Input Parameters
* `count` - _optional_ - Number of messages to return, between 1 and 1000.
* `unreads` - _optional_ - Include `unread_count_display` in the output?
* `inclusive` - _optional_ - Include messages with latest or oldest timestamp in results.
* `token` - _optional_ - Authentication token. Requires scope: `im:history`
* `oldest` - _optional_ - Start of time range of messages to include in results.
* `channel` - _optional_ - Direct message channel to fetch history for.
* `latest` - _optional_ - End of time range of messages to include in results.

### Lists direct message channels for the calling user.

*Tags:* `im`

#### Input Parameters
* `cursor` - _optional_ - Paginate through collections of data by setting the `cursor` parameter to a `next_cursor` attribute returned by a previous request's `response_metadata`. Default value fetches the first "page" of the collection. See [pagination](/docs/pagination) for more detail.
* `token` - _optional_ - Authentication token. Requires scope: `im:read`
* `limit` - _optional_ - The maximum number of items to return. Fewer than the requested number of items may be returned, even if the end of the users list hasn't been reached.

### Sets the read cursor in a direct message channel.

*Tags:* `im`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `im:write`

### Opens a direct message channel.

*Tags:* `im`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `im:write`

### Retrieve a thread of messages posted to a direct message conversation

*Tags:* `im`

#### Input Parameters
* `thread_ts` - _optional_ - Unique identifier of a thread's parent message
* `token` - _optional_ - Authentication token. Requires scope: `im:history`
* `channel` - _optional_ - Direct message channel to fetch thread from

### For Enterprise Grid workspaces, map local user IDs to global user IDs

*Tags:* `migration`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `tokens.basic`
* `to_old` - _optional_ - Specify `true` to convert `W` global user IDs to workspace-specific `U` IDs. Defaults to `false`.
* `users` - _optional_ - A comma-separated list of user ids, up to 400 per request

### Closes a multiparty direct message channel.

*Tags:* `mpim`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `mpim:write`

### Fetches history of messages and events from a multiparty direct message.

*Tags:* `mpim`

#### Input Parameters
* `count` - _optional_ - Number of messages to return, between 1 and 1000.
* `unreads` - _optional_ - Include `unread_count_display` in the output?
* `inclusive` - _optional_ - Include messages with latest or oldest timestamp in results.
* `token` - _optional_ - Authentication token. Requires scope: `mpim:history`
* `oldest` - _optional_ - Start of time range of messages to include in results.
* `channel` - _optional_ - Multiparty direct message to fetch history for.
* `latest` - _optional_ - End of time range of messages to include in results.

### Lists multiparty direct message channels for the calling user.

*Tags:* `mpim`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `mpim:read`

### Sets the read cursor in a multiparty direct message channel.

*Tags:* `mpim`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `mpim:write`

### This method opens a multiparty direct message.

*Tags:* `mpim`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `mpim:write`

### Retrieve a thread of messages posted to a direct message conversation from a multiparty direct message.

*Tags:* `mpim`

#### Input Parameters
* `thread_ts` - _optional_ - Unique identifier of a thread's parent message.
* `token` - _optional_ - Authentication token. Requires scope: `mpim:history`
* `channel` - _optional_ - Multiparty direct message channel to fetch thread from.

### Exchanges a temporary OAuth verifier code for an access token.

*Tags:* `oauth`

#### Input Parameters
* `client_secret` - _optional_ - Issued when you created your application.
* `code` - _optional_ - The `code` param returned via the OAuth callback.
* `single_channel` - _optional_ - Request the user to add your app only to a single channel.
* `client_id` - _optional_ - Issued when you created your application.
* `redirect_uri` - _optional_ - This must match the originally submitted URI (if one was sent).

### Exchanges a temporary OAuth verifier code for a workspace token.

*Tags:* `oauth`

#### Input Parameters
* `client_secret` - _optional_ - Issued when you created your application.
* `code` - _optional_ - The `code` param returned via the OAuth callback.
* `single_channel` - _optional_ - Request the user to add your app only to a single channel.
* `client_id` - _optional_ - Issued when you created your application.
* `redirect_uri` - _optional_ - This must match the originally submitted URI (if one was sent).

### Pins an item to a channel.

*Tags:* `pins`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `pins:write`

### Lists items pinned to a channel.

*Tags:* `pins`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `pins:read`
* `channel` - _optional_ - Channel to get pinned items for.

### Un-pins an item from a channel.

*Tags:* `pins`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `pins:write`

### Adds a reaction to an item.

*Tags:* `reactions`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `reactions:write`

### Gets reactions for an item.

*Tags:* `reactions`

#### Input Parameters
* `full` - _optional_ - If true always return the complete reaction list.
* `file_comment` - _optional_ - File comment to get reactions for.
* `timestamp` - _optional_ - Timestamp of the message to get reactions for.
* `token` - _optional_ - Authentication token. Requires scope: `reactions:read`
* `file` - _optional_ - File to get reactions for.
* `channel` - _optional_ - Channel where the message to get reactions for was posted.

### Lists reactions made by a user.

*Tags:* `reactions`

#### Input Parameters
* `count` - _optional_
* `token` - _optional_ - Authentication token. Requires scope: `reactions:read`
* `full` - _optional_ - If true always return the complete reaction list.
* `user` - _optional_ - Show reactions made by this user. Defaults to the authed user.
* `page` - _optional_

### Removes a reaction from an item.

*Tags:* `reactions`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `reactions:write`

### Creates a reminder.

*Tags:* `reminders`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `reminders:write`

### Marks a reminder as complete.

*Tags:* `reminders`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `reminders:write`

### Deletes a reminder.

*Tags:* `reminders`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `reminders:write`

### Gets information about a reminder.

*Tags:* `reminders`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `reminders:read`
* `reminder` - _optional_ - The ID of the reminder

### Lists all reminders created by or for a given user.

*Tags:* `reminders`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `reminders:read`

### Starts a Real Time Messaging session.

*Tags:* `rtm`

#### Input Parameters
* `presence_sub` - _optional_ - Only deliver presence events when requested by subscription. See [presence subscriptions](/docs/presence-and-status#subscriptions).
* `token` - _optional_ - Authentication token. Requires scope: `rtm:stream`
* `batch_presence_aware` - _optional_ - Batch presence deliveries via subscription. Enabling changes the shape of `presence_change` events. See [batch presence](/docs/presence-and-status#batching).

### Starts a Real Time Messaging session.

*Tags:* `rtm`

#### Input Parameters
* `no_latest` - _optional_ - Exclude latest timestamps for channels, groups, mpims, and ims. Automatically sets `no_unreads` to `1`
* `simple_latest` - _optional_ - Return timestamp only for latest message object of each channel (improves performance).
* `include_locale` - _optional_ - Set this to `true` to receive the locale for users and channels. Defaults to `false`
* `presence_sub` - _optional_ - Only deliver presence events when requested by subscription. See [presence subscriptions](/docs/presence-and-status#subscriptions).
* `no_unreads` - _optional_ - Skip unread counts for each channel (improves performance).
* `batch_presence_aware` - _optional_ - Batch presence deliveries via subscription. Enabling changes the shape of `presence_change` events. See [batch presence](/docs/presence-and-status#batching).
* `mpim_aware` - _optional_ - Returns MPIMs to the client in the API response.
* `token` - _optional_ - Authentication token. Requires scope: `rtm:stream`

### Searches for messages and files matching a query.

*Tags:* `search`

#### Input Parameters
* `sort_dir` - _optional_ - Change sort direction to ascending (`asc`) or descending (`desc`).
* `query` - _optional_ - Search query. May contains booleans, etc.
* `sort` - _optional_ - Return matches sorted by either `score` or `timestamp`.
* `count` - _optional_
* `token` - _optional_ - Authentication token. Requires scope: `search:read`
* `highlight` - _optional_ - Pass a value of `true` to enable query highlight markers (see below).
* `page` - _optional_

### Searches for files matching a query.

*Tags:* `search`

#### Input Parameters
* `sort_dir` - _optional_ - Change sort direction to ascending (`asc`) or descending (`desc`).
* `query` - _optional_ - Search query.
* `sort` - _optional_ - Return matches sorted by either `score` or `timestamp`.
* `highlight` - _optional_ - Pass a value of `true` to enable query highlight markers (see below).
* `count` - _optional_
* `token` - _optional_ - Authentication token. Requires scope: `search:read`
* `page` - _optional_

### Searches for messages matching a query.

*Tags:* `search`

#### Input Parameters
* `sort_dir` - _optional_ - Change sort direction to ascending (`asc`) or descending (`desc`).
* `query` - _optional_ - Search query.
* `sort` - _optional_ - Return matches sorted by either `score` or `timestamp`.
* `count` - _optional_ - Pass the number of results you want per "page". Maximum of `100`.
* `token` - _optional_ - Authentication token. Requires scope: `search:read`
* `highlight` - _optional_ - Pass a value of `true` to enable query highlight markers (see below).
* `page` - _optional_

### Adds a star to an item.

*Tags:* `stars`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `stars:write`

### Lists stars for a user.

*Tags:* `stars`

#### Input Parameters
* `count` - _optional_
* `token` - _optional_ - Authentication token. Requires scope: `stars:read`
* `page` - _optional_

### Removes a star from an item.

*Tags:* `stars`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `stars:write`

### Gets the access logs for the current team.

*Tags:* `team`

#### Input Parameters
* `count` - _optional_
* `token` - _optional_ - Authentication token. Requires scope: `admin`
* `page` - _optional_
* `before` - _optional_ - End of time range of logs to include in results (inclusive).

### Gets billable users information for the current team.

*Tags:* `team`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `admin`
* `user` - _optional_ - A user to retrieve the billable information for. Defaults to all users.

### Gets information about the current team.

*Tags:* `team`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `team:read`

### Gets the integration logs for the current team.

*Tags:* `team`

#### Input Parameters
* `count` - _optional_
* `change_type` - _optional_ - Filter logs with this change type. Defaults to all logs.
* `app_id` - _optional_ - Filter logs to this Slack app. Defaults to all logs.
* `token` - _optional_ - Authentication token. Requires scope: `admin`
* `user` - _optional_ - Filter logs generated by this user's actions. Defaults to all logs.
* `service_id` - _optional_ - Filter logs to this service. Defaults to all logs.
* `page` - _optional_

### Retrieve a team's profile.

*Tags:* `team.profile` `team`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `users.profile:read`
* `visibility` - _optional_ - Filter by visibility.

### Create a User Group

*Tags:* `usergroups`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `usergroups:write`

### Disable an existing User Group

*Tags:* `usergroups`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `usergroups:write`

### Enable a User Group

*Tags:* `usergroups`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `usergroups:write`

### List all User Groups for a team

*Tags:* `usergroups`

#### Input Parameters
* `include_users` - _optional_ - Include the list of users for each User Group.
* `token` - _optional_ - Authentication token. Requires scope: `usergroups:read`
* `include_count` - _optional_ - Include the number of users in each User Group.
* `include_disabled` - _optional_ - Include disabled User Groups.

### Update an existing User Group

*Tags:* `usergroups`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `usergroups:write`

### List all users in a User Group

*Tags:* `usergroups.users` `usergroups`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `usergroups:read`
* `include_disabled` - _optional_ - Allow results that involve disabled User Groups.
* `usergroup` - _optional_ - The encoded ID of the User Group to update.

### Update the list of users for a User Group

*Tags:* `usergroups.users` `usergroups`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `usergroups:write`

### List conversations the calling user may access.

*Tags:* `users`

#### Input Parameters
* `cursor` - _optional_ - Paginate through collections of data by setting the `cursor` parameter to a `next_cursor` attribute returned by a previous request's `response_metadata`. Default value fetches the first "page" of the collection. See [pagination](/docs/pagination) for more detail.
* `token` - _optional_ - Authentication token. Requires scope: `conversations:read`
* `limit` - _optional_ - The maximum number of items to return. Fewer than the requested number of items may be returned, even if the end of the list hasn't been reached. Must be an integer no larger than 1000.
* `user` - _optional_ - Browse conversations by a specific user ID's membership. Non-public channels are restricted to those where the calling user shares membership.
* `exclude_archived` - _optional_ - Set to `true` to exclude archived channels from the list
* `types` - _optional_ - Mix and match channel types by providing a comma-separated list of any combination of `public_channel`, `private_channel`, `mpim`, `im`

### Delete the user profile photo

*Tags:* `users`

### Gets user presence information.

*Tags:* `users`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `users:read`
* `user` - _optional_ - User to get presence info on. Defaults to the authed user.

### Get a user's identity.

*Tags:* `users`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `identity.basic`

### Gets information about a user.

*Tags:* `users`

#### Input Parameters
* `include_locale` - _optional_ - Set this to `true` to receive the locale for this user. Defaults to `false`
* `token` - _optional_ - Authentication token. Requires scope: `users:read`
* `user` - _optional_ - User to get info on

### Lists all users in a Slack team.

*Tags:* `users`

#### Input Parameters
* `presence` - _optional_ - Deprecated. Whether to include presence data in the output. Defaults to `false`. Setting this to `true` reduces performance, especially with large teams.
* `cursor` - _optional_ - Paginate through collections of data by setting the `cursor` parameter to a `next_cursor` attribute returned by a previous request's `response_metadata`. Default value fetches the first "page" of the collection. See [pagination](/docs/pagination) for more detail.
* `token` - _optional_ - Authentication token. Requires scope: `users:read`
* `limit` - _optional_ - The maximum number of items to return. Fewer than the requested number of items may be returned, even if the end of the users list hasn't been reached.
* `include_locale` - _optional_ - Set this to `true` to receive the locale for users. Defaults to `false`

### Find a user with an email address.

*Tags:* `users`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `users:read.email`
* `email` - _optional_ - An email address belonging to a user in the workspace

### Retrieves a user's profile information.

*Tags:* `users.profile` `users`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `users.profile:read`
* `include_labels` - _optional_ - Include labels for each ID in custom profile fields
* `user` - _optional_ - User to retrieve profile info for

### Set the profile information for a user.

*Tags:* `users.profile` `users`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `users.profile:write`

### Marked a user as active. Deprecated and non-functional.

*Tags:* `users`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `users:write`

### Set the user profile photo

*Tags:* `users`

### Manually sets user presence.

*Tags:* `users`

#### Input Parameters
* `token` - _optional_ - Authentication token. Requires scope: `users:write`

## License

**flow**ground :- Telekom iPaaS / slack-com-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
