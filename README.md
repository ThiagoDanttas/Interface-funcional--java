# Interface funcional - java

---

� uma interface que possui um �nico m�todo abstrato. Suas
implementa��es ser�o tratadas como express�es lambda.

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