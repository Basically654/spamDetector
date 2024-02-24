import java.io.File;
import java.io.FileNotFoundException;
import java.util.ArrayList;
import java.util.Scanner;
public class fileReader {
    public static void main(String[] args){
        /*If the while loop detects matching keyword from spam list
        it should stop and check if the rest of the phrase matches as well.
         */
        try{
            File myObj = new File("spamList.txt");
            File mySpam = new File("spam.txt");
            ArrayList<String> spamList = new ArrayList<>();
            ArrayList<String> spamText = new ArrayList<>();
            Scanner myReader = new Scanner(myObj);
            int spamCheck = 0;
            while (myReader.hasNextLine()) {
                while (myReader.hasNext()){
                    spamList.add(myReader.nextLine());
                    spamList.replaceAll(String::toUpperCase);
                }
                ///System.out.println(spamList);
            }
            Scanner spamReader = new Scanner(mySpam);
            while(spamReader.hasNextLine()){
                while(spamReader.hasNext()){
                    spamText.add(spamReader.nextLine());
                    spamText.replaceAll(String::toUpperCase);
                    for(String textSpam: spamText) {
                        for(String listSpam: spamList){
                            if(textSpam.contains(listSpam)){
                                spamCheck += 1;
                            }
                        }
                    }
                }
                if(spamCheck >= 1){
                    System.out.println("This could potentially be spam.");
                }else{
                    System.out.println("Looks good!");
                }
                //System.out.println(spamText);
            }myReader.close();
        }catch (FileNotFoundException e){
            System.out.println("File not found.");
        }
    }
}
