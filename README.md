[11/07, 11:22 am] Ashwin Friend Viswa: import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int n = sc.nextInt();
        int sum = 0;

        for (int i = 0; i < n; i++) {
            int num = sc.nextInt();
            if (num > 0) {
                sum += num * num;
            }
        }

        System.out.println("Sum of positive square elements: " + sum);

        sc.close();
    }
}
[11/07, 11:22 am] Ashwin Friend Viswa: import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        String str = sc.nextLine();
        StringBuilder result = new StringBuilder();

        for (int i = 0; i < str.length(); i++) {
            result.append(str.charAt(i));
            if (i < str.length() - 1 && str.charAt(i) == str.charAt(i + 1)) {
                result.append("*");
            }
        }

        System.out.println(result.toString());

        sc.close();
    }
}
[11/07, 11:22 am] Ashwin Friend Viswa: import java.util.*;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int n = sc.nextInt();
        TreeMap<Integer, Integer> map = new TreeMap<>();

        for (int i = 0; i < n; i++) {
            int num = sc.nextInt();
            map.put(num, map.getOrDefault(num, 0) + 1);
        }

        System.out.println("Frequency of each element in the array:");
        for (Map.Entry<Integer, Integer> entry : map.entrySet()) {
            System.out.println(entry.getKey() + ": " + entry.getValue());
        }

        sc.close();
    }
}