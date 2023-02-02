# Interface funcional - java

---

É uma interface que possui um único método abstrato. Suas
implementações serão tratadas como expressões lambda.

~~~~java 
public class MyComparator implements Comparator<Product> {

    @Override
    public int compare(Product p1, Product p2) {
        return p1.getName().toUpperCase().compareTo(p2.getName().toUpperCase());
    }
}

~~~~

~~~~java
public static void main(String[] args){
    //(...)
    list.sort(new MyComparator());
}
~~~~