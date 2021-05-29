# Week-4-Coding-Assignment
import java.util.HashSet;
import java.util.ArrayList;
import java.util.List;
import java.util.Set;
import java.util.Map;
import java.util.HashMap;

public class App {
    public static void main(String[] args) throws Exception {

        // Question 1
        List<String> employeeNames = new ArrayList<String>();
        employeeNames.add("Eddy");
        employeeNames.add("Sean");
        employeeNames.add("Bob");
        employeeNames.add("Andrew");

        for (int i = 0; i < employeeNames.size(); i++) {
            System.out.println(employeeNames.get(i));
        }

        // Question 2
        Set<Integer> ids = new HashSet<Integer>();
        ids.add(14);
        ids.add(23);
        ids.add(32);
        ids.add(65);

        System.out.println(ids);

        // Question 3 and 4
        Map<Integer, String> employeeMap = new HashMap<Integer, String>();
        employeeMap.put(1, "Office");
        employeeMap.put(2, "Lounge");
        employeeMap.put(3, "Cafeteria");
        employeeMap.put(3, "Lunch");

        // Question 5
        int i = 0;
        for (int id : ids) {
            employeeMap.put(id, employeeMap.get(i++));
        }
        // Question 6
        for (int id : employeeMap.keySet()) {
            System.out.println(employeeMap.get(id));
        }

        // Question 7-9
        StringBuilder idsBuilder = new StringBuilder();

        for (int id : ids) {
            idsBuilder.append(id + "-");
        }
        System.out.println(idsBuilder.toString());

        // Question 10-12
        StringBuilder namesBuilder = new StringBuilder();

        for (String names : employeeNames) {
            namesBuilder.append(names + " ");
        }
        System.out.println(namesBuilder.toString());

    }

}
