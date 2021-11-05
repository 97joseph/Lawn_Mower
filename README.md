# Lawn_Mower

Abstractive methods


## Engine Class

| Engine                                                                                |
| ------------------------------------------------------------------------------------- |
| -manufacturer : String-horsePower : double-cylinders : integer                        |
| +Engine()+Engine( //all Engine properties )+//Accessor and Mutators+toString():String |

## *Mower Class* (Abstract)

| *Mower*                                                           |
| ------------------------------------------------------------------- |
| -manufacturer : String-year : integer-serialNumber : String         |
| +Mower()+Mower( //All properties )+//Getters and setters+toString() |

## LawnTractor Class

This class will define each grade level that can be obtained in the course (D to A).

| LawnTractor                                              |
| -------------------------------------------------------- |
| -engine : Engine-model : String-deckWidth : double       |
| +LawnTractor()+//Accessor and Mutators+toString():String |

## CommercialMower Class

This class will track the points received and the maximum points for each class assignment.

| CommercialMower                                              |
| ------------------------------------------------------------ |
| -operatingHours : double-zeroTurnRadius : boolean            |
| +CommercialMower()+//Accessor and Mutators+toString():String |

## *WalkBehindMower* Class (Abstract)

| *WalkBehindMower*                                          |
| ------------------------------------------------------------ |
| -cutWidth : double-wheelDiameter : double                    |
| +WalkBehindMower()+//Accessor and Mutators+toString():String |

## GasPoweredMower

| GasPoweredMower                                             |
| ----------------------------------------------------------- |
| -engine : Engine-selfPropelled : boolean                    |
| GasPoweredMower()+//Accessor and Mutators+toString():String |

## PushReelMower

| PushReelMower                                              |
| ---------------------------------------------------------- |
| -numWheels : integer                                       |
| +PushReelMower()+//Accessor and Mutators+toString():String |

## MowerWareHouse

| MowerWareHouse                                                                                                                                        |
| ----------------------------------------------------------------------------------------------------------------------------------------------------- |
| -storeName : String-mowers : ArrayList`<Mower>`                                                                                                     |
| +MowerWareHouse()+//Accessor and Mutators+readMowerData( inputFileName : String) : void+saveMowerData( outputFileName :String):void+toString():String |

# Handling ArrayLists

Each ArrayList should have five associated methods to perform: getNum, add, remove, get and set. So if you have an ArrayList named *widgets* that stored items of type Widget, then the associated UML behaviors would be:

+getNumWidget **s** () : int //Return the number of items in the ArrayList widgets.

+getWidget(index:int) : Widget //get the Widget at location index in ArrayList widgets

+setWidget(index:int, item:Widget):void //store item at location index in the ArrayList widgets.

+addWidget(item:Widget):void //Append the Widget to the ArrayList.

+removeWidget( index:int ) : Widget //remove and return the Widget at location index

# Input File

The name of the input file will be supplied using command-line arguments. If no command-line argument is supplied, then your program should prompt the user for the input file using the JFileChooser class. Here is the format of the input file:

Store name

Mower Class Properties

Mower Subclass Type (L, C, G, P)

Subclass Properties

Note: Each properties will be on a separate line in the same order listed in the UML diagrams.

# Output File

The format for the output file should be identical to that of the input file. In other words, after writing your output file, you should be able to read it back in as an input file. The toString() methods of your classes are designed to make file output simple.

Figure 1: Input File Format

# Graphical User Interface

**Viewing:** The View window should display the name of each type of concrete mower (LawnTractor, CommericalMower, GasPoweredMower and PushReelMower). Also include a JButton next to each of these mower types that will initiate the population of a JList showing all the properties of each mower of that type. The JList can be included on the View window or as a separate JDialog.
