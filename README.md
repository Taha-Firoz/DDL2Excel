# Oracle SQL DDL to Excel

This script converts any Oracle SQL DDL commands into Table headings and columns to allow for easy creation of Datasets

## Getting Started

You'll need Python3 and OpenPyxl

### Prerequisites

You can install OpenPyxl with pip like this

```
pip install openpyxl --user
```

### Installing

To start of copy your ddl commands into a textfile.
Then run the commans

```
python3 DDL2Excel [Filename.txt] [Outputfile.xlsx]
```
Replace [Filename.txt] with the included "test.txt" file and [Outputfile.xlsx] with "Outputfile.xlsx"
Like so
```
python3 DDL2Excel text.txt Outputfile.xlsx
```
If the code runs successfully you should have an Outputfile.xlsx in your directory


### Changing Colours of filled blocks

If you wish to change the colour of the filled blocks you can change the values of ```table_heading``` and ```table_columns```

```
table_heading = PatternFill(start_color='FF6AA84F',
                        end_color='FF6AA84F',
                        fill_type='solid')
```
Add the hexcode of the colour you wish to choose into the ```start_color``` and ```end_color``` parameters.
The first two letters as is and append your 6 digit hexcode to them e.g. Dark Green  has a  hex code "6AA84F"
so we'll set the start_color to 
```
start_color = 'FF' + '6AA84F',
end_color = 'FF' + '6AA84F'
```

## Built With

* [Python3](https://www.python.org/) - The Language Used
* [OpenPyxl](https://openpyxl.readthedocs.io/en/stable/) - The Library Used


## Authors

* **Mohammad Taha Bin Firoz** - [Taha Firoz](https://github.com/Taha-Firoz)
* **Mohammad Ziad Siddiqui** - [Ziad Coolio](https://github.com/ziadcoolio)

See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.

## License

This project is licensed under the GPL V3 License - see the [LICENSE.md](LICENSE.md) file for details

