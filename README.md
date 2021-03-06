# Metrixpp To JSON

This is a tool that helps you to make a json output from a metrix++ CSV file.

## Usage

Use the following maven command to build this project `mvn clean install`.

Then, you can run this tool and output the results in the stdout or in a json file.

Let's see what we get for the following CSV input file. 
You can make a file like this by running metrix++ on this project.
I will run; 

`java -DinputCSV="path/to/your/input.csv" -DoutputJson="path/to/your/output.json" -jar target/metrix2json-jar-with-dependencies.jar`

NOTE: keep in mind to add `-jar target/metrix2json-jar-with-dependencies.jar` at the end.

```csv
file,region,type,modified,line start,line end,std.code.complexity:cyclomatic,std.code.complexity:maxindent,std.code.lines:code,std.code.lines:preprocessor,std.code.lines:comments,std.code.mi:simple,std.code.member:globals
./src/main/java/org/dxworks/metrix2json/Entity/Metrix2JsonOutput.java,__global__,global,,1,49,,,4,0,0,1,
./src/main/java/org/dxworks/metrix2json/Entity/Metrix2JsonOutput.java,Metrix2JsonOutput,class,,8,48,,,12,0,0,1,
./src/main/java/org/dxworks/metrix2json/Entity/Metrix2JsonOutput.java,buildOutput,function,,25,47,1,2,18,0,0,1,
./src/main/java/org/dxworks/metrix2json/Entity/Metrix2JsonOutput.java,,file,,1,49,,,,,,,
./src/main/java/org/dxworks/metrix2json/Entity/MetrixppOutput.java,__global__,global,,1,76,,,7,0,0,1,
./src/main/java/org/dxworks/metrix2json/Entity/MetrixppOutput.java,MetrixppOutput,class,,11,75,,,32,0,0,1,
./src/main/java/org/dxworks/metrix2json/Entity/MetrixppOutput.java,unify,function,,56,74,0,1,19,0,0,1,
./src/main/java/org/dxworks/metrix2json/Entity/MetrixppOutput.java,,file,,1,76,,,,,,,
./src/main/java/org/dxworks/metrix2json/Entity/UnifiableOutput.java,__global__,global,,1,8,,,1,0,0,1,
./src/main/java/org/dxworks/metrix2json/Entity/UnifiableOutput.java,UnifiableOutput,interface,,3,7,,,3,0,0,1,
./src/main/java/org/dxworks/metrix2json/Entity/UnifiableOutput.java,,file,,1,8,,,,,,,
./src/main/java/org/dxworks/metrix2json/Entity/UnifiedOutput.java,__global__,global,,1,55,,,3,0,0,1,
./src/main/java/org/dxworks/metrix2json/Entity/UnifiedOutput.java,UnifiedOutput,class,,7,54,,,27,0,0,1,
./src/main/java/org/dxworks/metrix2json/Entity/UnifiedOutput.java,,file,,1,55,,,,,,,
./src/main/java/org/dxworks/metrix2json/Metrix2Json.java,__global__,global,,1,68,,,8,0,0,1,
./src/main/java/org/dxworks/metrix2json/Metrix2Json.java,Metrix2Json,class,,12,67,,,2,0,0,1,
./src/main/java/org/dxworks/metrix2json/Metrix2Json.java,main,function,,14,39,3,3,20,0,0,1,
./src/main/java/org/dxworks/metrix2json/Metrix2Json.java,getOutputPath,function,,41,52,1,2,8,0,0,1,
./src/main/java/org/dxworks/metrix2json/Metrix2Json.java,getInputPath,function,,54,65,1,2,8,0,0,1,
./src/main/java/org/dxworks/metrix2json/Metrix2Json.java,,file,,1,68,,,,,,,
./src/main/java/org/dxworks/metrix2json/Process/ProcessMetrixppOutput.java,__global__,global,,1,38,,,6,0,0,1,
./src/main/java/org/dxworks/metrix2json/Process/ProcessMetrixppOutput.java,ProcessMetrixppOutput,class,,10,37,,,2,0,0,1,
./src/main/java/org/dxworks/metrix2json/Process/ProcessMetrixppOutput.java,processMatrixpp,function,,12,35,2,3,19,0,0,1,
./src/main/java/org/dxworks/metrix2json/Process/ProcessMetrixppOutput.java,,file,,1,38,,,,,,,
./src/main/java/org/dxworks/metrix2json/Reader/CSVFileReader.java,__global__,global,,1,26,,,7,0,0,1,
./src/main/java/org/dxworks/metrix2json/Reader/CSVFileReader.java,CSVFileReader,class,,11,25,,,2,0,0,1,
./src/main/java/org/dxworks/metrix2json/Reader/CSVFileReader.java,CSVFileReader,function,,13,13,0,1,1,0,0,1,
./src/main/java/org/dxworks/metrix2json/Reader/CSVFileReader.java,readCSV,function,,15,23,0,1,7,0,0,1,
./src/main/java/org/dxworks/metrix2json/Reader/CSVFileReader.java,,file,,1,26,,,,,,,
./src/main/java/org/dxworks/metrix2json/Reader/FileReader.java,__global__,global,,1,13,,,5,0,0,1,
./src/main/java/org/dxworks/metrix2json/Reader/FileReader.java,FileReader,interface,,9,12,,,3,0,0,1,
./src/main/java/org/dxworks/metrix2json/Reader/FileReader.java,,file,,1,13,,,,,,,
./src/main/java/org/dxworks/metrix2json/Reader/MetrixppCSVFileReader.java,__global__,global,,1,23,,,5,0,0,1,
./src/main/java/org/dxworks/metrix2json/Reader/MetrixppCSVFileReader.java,MetrixppCSVFileReader,class,,9,22,,,3,0,0,1,
./src/main/java/org/dxworks/metrix2json/Reader/MetrixppCSVFileReader.java,MetrixppCSVFileReader,function,,11,11,0,1,1,0,0,1,
./src/main/java/org/dxworks/metrix2json/Reader/MetrixppCSVFileReader.java,getInstance,function,,15,17,0,1,3,0,0,1,
./src/main/java/org/dxworks/metrix2json/Reader/MetrixppCSVFileReader.java,readFileCSV,function,,19,21,0,1,3,0,0,1,
./src/main/java/org/dxworks/metrix2json/Reader/MetrixppCSVFileReader.java,,file,,1,23,,,,,,,
```  