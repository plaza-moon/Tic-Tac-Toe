import java.util.Scanner;

public class tictactoe {
    private static int countChar(String str, char c)
    {
        int count = 0;

        for(int i=0; i < str.length(); i++)
        {    if(str.charAt(i) == c)
            count++;
        }

        return count;
    }
    public static void main(String[] args) {
        char[] inputArr = new char[]{' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' '};
        String start = "| ";
        String end = " |";

        System.out.println("---------");
        System.out.println(start + inputArr[0] + " " + inputArr[1] + " " + inputArr[2] + end);
        System.out.println(start + inputArr[3] + " " + inputArr[4] + " " + inputArr[5] + end);
        System.out.println(start + inputArr[6] + " " + inputArr[7] + " " + inputArr[8] + end);
        System.out.println("---------");

        char Y = 'Y';
        for (int i=0; i < inputArr.length; i++) {
            if (i%2 == 0) {
                Y = 'X';
            } else {
                Y = 'O';
            }
            boolean a = true;
            while (a) {
                System.out.print("Enter the coordinates: ");
                Scanner scanner2 = new Scanner(System.in);
                try {
                    int first = scanner2.nextInt();
                    int second = scanner2.nextInt();
                    if ((first == 1 & second == 1) | (first == 2 & second == 1) | (first == 3 & second == 1) |
                            (first == 1 & second == 2) | (first == 2 & second == 2) | (first == 3 & second == 2) |
                            (first == 1 & second == 3) | (first == 2 & second == 3) | (first == 3 & second == 3)) {
                        if (first == 1 & second == 1 & inputArr[6] == ' ') {
                            inputArr[6] = Y;
                            a = false;
                        } else if (first == 2 & second == 1 & inputArr[7] == ' ') {
                            inputArr[7] = Y;
                            a = false;
                        } else if (first == 3 & second == 1 & inputArr[8] == ' ') {
                            inputArr[8] = Y;
                            a = false;
                        } else if (first == 1 & second == 2 & inputArr[3] == ' ') {
                            inputArr[3] = Y;
                            a = false;
                        } else if (first == 2 & second == 2 & inputArr[4] == ' ') {
                            inputArr[4] = Y;
                            a = false;
                        } else if (first == 3 & second == 2 & inputArr[5] == ' ') {
                            inputArr[5] = Y;
                            a = false;
                        } else if (first == 1 & second == 3 & inputArr[0] == ' ') {
                            inputArr[0] = Y;
                            a = false;
                        } else if (first == 2 & second == 3 & inputArr[1] == ' ') {
                            inputArr[1] = Y;
                            a = false;
                        } else if (first == 3 & second == 3 & inputArr[2] == ' ') {
                            inputArr[2] = Y;
                            a = false;
                        } else {
                            System.out.println("This cell is occupied! Choose another one!");
                        }
                    } else {
                        System.out.println("Coordinates should be from 1 to 3!");
                    }
                } catch (Exception e) {
                    System.out.println("You should enter numbers!");
                    scanner2.next(); // clear scanner wrong input
                    continue;
                }
            }
            System.out.println("---------");
            System.out.println(start + inputArr[0] + " " + inputArr[1] + " " + inputArr[2] + end);
            System.out.println(start + inputArr[3] + " " + inputArr[4] + " " + inputArr[5] + end);
            System.out.println(start + inputArr[6] + " " + inputArr[7] + " " + inputArr[8] + end);
            System.out.println("---------");

            String inputArr2 = new String(inputArr);
            if ((inputArr[0] == 'X' && inputArr[0] == inputArr[1] && inputArr[1] == inputArr[2]) ||
                    (inputArr[3] == 'X' && inputArr[3] == inputArr[4] && inputArr[4] == inputArr[5]) ||
                    (inputArr[6] == 'X' && inputArr[6] == inputArr[7] && inputArr[7] == inputArr[8]) ||

                    (inputArr[0] == 'X' && inputArr[0] == inputArr[4] && inputArr[4] == inputArr[8]) ||
                    (inputArr[2] == 'X' && inputArr[2] == inputArr[4] && inputArr[4] == inputArr[6]) ||

                    (inputArr[0] == 'X' && inputArr[0] == inputArr[3] && inputArr[3] == inputArr[6]) ||
                    (inputArr[1] == 'X' && inputArr[1] == inputArr[4] && inputArr[4] == inputArr[7]) ||
                    (inputArr[2] == 'X' && inputArr[2] == inputArr[5] && inputArr[5] == inputArr[8])) {

                System.out.println("X wins");
                break;
            }
            else if ((inputArr[0] == 'O' && inputArr[0] == inputArr[1] && inputArr[1] == inputArr[2]) ||
                    (inputArr[3] == 'O' && inputArr[3] == inputArr[4] && inputArr[4] == inputArr[5]) ||
                    (inputArr[6] == 'O' && inputArr[6] == inputArr[7] && inputArr[7] == inputArr[8]) ||

                    (inputArr[0] == 'O' && inputArr[0] == inputArr[4] && inputArr[4] == inputArr[8]) ||
                    (inputArr[2] == 'O' && inputArr[2] == inputArr[4] && inputArr[4] == inputArr[6]) ||

                    (inputArr[0] == 'O' && inputArr[0] == inputArr[3] && inputArr[3] == inputArr[6]) ||
                    (inputArr[1] == 'O' && inputArr[1] == inputArr[4] && inputArr[4] == inputArr[7]) ||
                    (inputArr[2] == 'O' && inputArr[2] == inputArr[5] && inputArr[5] == inputArr[8])) {

                System.out.println("O wins");
                break;
            } else if ((countChar(inputArr2, 'X') == 5 && countChar(inputArr2, 'O') == 4) ||
                    (countChar(inputArr2, 'X') == 4 && countChar(inputArr2, 'O') == 5)) {

                System.out.println("Draw");
                break;
            }
        }
    }
}
