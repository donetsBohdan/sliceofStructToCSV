{\rtf1\ansi\deff0\nouicompat{\fonttbl{\f0\fnil\fcharset0 Courier New;}}
{\*\generator Riched20 10.0.16299}\viewkind4\uc1 
\pard\b\f0\fs22\lang1033 sliceOfStructToCSV\b0\par
SliceofStructToCSV is very simple library to wrtie CSV files from slice of structs without setting a type of struct. \par
\par
It uses reflect package, gets names of struct's fields and write them to the title of bytes.Buffer, values of fields are written to body. Also you can add to each field tag "title" to replace title of csv to these tags. The only thing you should do is to append all structs to the slice of interface and use func GetCSV(). Maybe in future I'll figure out how to do it simpler.\par
\par
All values are written as strings. For this purpose I used package "github.com/spf13/cast".\par
\par
\b Usage\b0\par
\par
Just use this:\par
\par
sliceOfStructToCSV.GetCSV(yourSlice []interface\{\}) *bytes.Buffer\par
}
 