[!!User Interface Channels](../UserInterface/02e_Channels.md)
[!!Configure the channel settings](../../PIM/Integration/ConfigureChannels.md)


# Manage the channels

A channel is needed to create offers for a certain connection. By default, the *Actindo Basic* channel is preset. If you want to maintain multiple channels, you have to create and activate the respective channels.

> [Info] A channel is not equal to a marketplace or web store connection. You can create a channel and use it for another connection.

[comment]: <> (Insert link for procedure about creating a new connection when available)

## Create a channel

Create a channel to maintain multiple channels or to create a new connection via the new channel.

#### Prerequisites

No prerequisites to fulfill.

#### Procedure
*DataHub > Settings > Tab CHANNELS*

![Channel list](../../Assets/Screenshots/DataHub/Settings/Channels/ChannelList.png "[Channel list]")

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
  The *Create channel* view is displayed.

  ![Create channel](../../Assets/Screenshots/DataHub/Settings/Channels/CreateChannel.png "[Create channel]")

2. Enter a name for the channel in the *Name* field and, if desired, add a channel description in the  *Description* field.

3. Enter a key for the channel in the *Key* field. The key is required for API access and must be system wide unique.

4. Enable the *Active* toggle to set the channel directly after creation to active.

  > [Info] The channel must be activated to be used.

5. Click the [SAVE] button in the upper right corner.   
  The new channel is saved. The *Create channel* view is closed.  



## Edit a channel

After you have created a channel, you can edit its name, description and key.

#### Prerequisites

At least one channel is created, see [Create a channel](../Integration/CreateChannel.md).

> [Info] By default, the *Actindo Basic* channel is created.

#### Procedure
*DataHub > Settings > Tab CHANNELS*

![Channel list](../../Assets/Screenshots/DataHub/Settings/Channels/ChannelList.png "[Channel list]")

1. Click the channel you want to edit in the list of channels.   
  The *Edit channel* view is displayed.

  ![Edit channel](../../Assets/Screenshots/DataHub/Settings/Channels/EditChannel.png "[Edit channel]")

2. Edit the desired data of the channel in the corresponding fields.

3. Click the [SAVE] button in the upper right corner.   
  The changes are saved. The *Edit channel* view is closed.  



## Deactivate a channel

Deactivate a channel when it should not be used for a certain time. The channel is no longer available for offers when it is inactive. Further, it is recommended to deactivate a channel instead of deleting it to prevent any problems because of existing connections.

#### Prerequisites

At least one channel is created, see [Create a channel](#create-a-channel).

> [Info] By default, the *Actindo Basic* channel is created.

#### Procedure
*DataHub > Settings > Tab CHANNELS*

![Channel list](../../Assets/Screenshots/DataHub/Settings/Channels/ChannelList.png "[Channel list]")

1. Click the channel you want to edit in the list of channels.   
  The *Edit channel* view is displayed.

  ![Edit channel](../../Assets/Screenshots/DataHub/Settings/Channels/EditChannel.png "[Edit channel]")

2. Disable the *Active* toggle.

3. Click the [SAVE] button in the upper right corner.   
  The channel is deactivated. The *Edit channel* view is closed.



## Delete a channel

You can delete a channel if it is no longer needed. As there are usually existing connections via a channel, it is highly recommended not to delete a channel. Instead, you can deactivate a channel and thus prevent its use.

#### Prerequisites

At least one channel is created, see [Create a channel](#create-a-channel).

> [Info] By default, the *Actindo Basic* channel is created. The *Actindo Basic* channel cannot be deleted.

#### Procedure
*DataHub > Settings > Tab CHANNELS*

![Channel list](../../Assets/Screenshots/DataHub/Settings/Channels/ChannelList.png "[Channel list]")

1. Select the checkbox of the channel you want to delete in the list of channels.    
  The editing toolbar is displayed above the channel list.

2. Click the [DELETE] button in the toolbar.  
  The channel is deleted. The deletion cannot be undone.

  > [Info] If the selected channel cannot be deleted, an error message is displayed in the upper right corner. To prevent the channels use, it is recommended to [deactivate the channel](#deactivate-a-channel) instead of delete it.
