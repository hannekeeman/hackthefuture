# Challenge 4 - Azure Logic Apps

Azure Logic Apps is a cloud-based platform for creating and running automated workflows that integrate your apps, data, services, and systems. With this platform, you can quickly develop highly scalable integration solutions for your enterprise and business-to-business. As a member of Azure Integration Services, Azure Logic Apps simplifies the way that you connect legacy, modern, and cutting-edge systems across cloud, on premises, and hybrid environments


## Instructions for Jill

JILL!!
WE NEED YOUR HELP TO STOP THAT MISSILE ASAP!!!! 

We did not expect it to be necessary to the fix the countdown logic so soon.
Anyway, in order to get it working you will have to create some logic that counts back from 10 to 0.

For each decrement, that url we gave you for must be called with the correct payload. (`HTTP POST`)

```json
{
  "teamId": "YOURTEAMID",
  "countdownNumber": 10
}
```
and then
```json
{
  "teamId": "YOURTEAMID",
  "countdownNumber": 9
}
```
And so on...

When you succesfully counted down from 10 to 0, our own missile will have successfully destroyed the target.

Go to the Azure Portal and check out the Logic App in the rg-challenge-4 resource group. \
Click on Logic App Designer.

Now create that looping logic that decrements the COUNTDOWN variable **until** it reaches 9 and do a HTTP POST call in each iteration.
