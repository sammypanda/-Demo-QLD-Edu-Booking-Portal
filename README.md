# (Demo) QLD Edu Booking Portal
A Demo developed with a self-administered two day deadline, shows my capacity to independently work with Microsoft Power Apps. Exported with built-in 'Export a solution'.

For educational purposes.

Index of objects in the demo:
![List of objects in the demo Power Apps solution](docs/assets/AllObjects.png)

## Booking Portal (Canvas)
![Start page (Main) of the canvas app](docs/assets/CanvasAppMain.png)
![Gallery page of bookable assets in the canvas app](docs/assets/CanvasAppBookableAssets.png)

## Tables
Truncated complexity to focus on an MVP.
### Asset
![The assets table, including a foreign key for Location](docs/assets/TableAsset.png)
### Location
![The locations table, including a foreign key for Created By](docs/assets/TableLocation.png)

## Dataverse
How the app components connect.

## Power Automation
### Blank Booker When Assets Not In Use
1. triggers on Asset table modify
2. for the modified rows, filters for not 'In Use' (status=1)
3. moves the current booker to 'Last Booker' column
4. nullifies the current booker in the 'Booker' column

![A snapshot of the code view of the data flow](docs/assets/AutomationBlankTheBooker.png)