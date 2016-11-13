# tamirinta7


public class tamirinta7 {

    public static void main(String args[]) {
        System.out.println("unique : " + numUnique(18, 3, 4));
        System.out.println("unique : " + numUnique(6, 7, 7));
    }

    public static int numUnique(int a, int b, int c) {
        int tmp = 0;
        //similar with triangle type check
        if (a == b && a == c) {
            tmp = 1;
        } //isosceles
        else if ((a == b && b != c)
                || (a == c && c != b)
                || (b == c && a != c)) {
            tmp = 2;
        } //scalene
        else {
            tmp = 3;
        }
        return tmp;
    }
}
