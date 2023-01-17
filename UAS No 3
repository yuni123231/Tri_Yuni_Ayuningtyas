import java.util.ArrayList;
import java.util.Scanner;

public class Belanja {
    private String NamaBarang;

    public String getNamaBarang() {
        return NamaBarang;
    }

    public void setNamaBarang(String namaBarang) {
        NamaBarang = namaBarang;
    }

    public int getHargaBarang() {
        return HargaBarang;
    }

    public void setHargaBarang(int hargaBarang) {
        HargaBarang = hargaBarang;
    }

    public int getJumBelanja() {
        return JumBelanja;
    }

    public void setJumBelanja(int jumBelanja) {
        JumBelanja = jumBelanja;
    }

    private int HargaBarang;
    private int JumBelanja;

    public ArrayList<Belanja> getItemSell() {
        return ItemSell;
    }

    public void setItemSell(ArrayList<Belanja> itemSell) {
        ItemSell = itemSell;
    }

    private ArrayList<Belanja> ItemSell;
    public Belanja(){

    }

    public void CetakInvoice(ArrayList<Belanja> Total) {
        for (int index = 0; index < Total.size(); index++){
            System.out.println(Total.get(index).getNamaBarang());
            System.out.println(Total.get(index).getHargaBarang() * getJumBelanja());
            System.out.println();
        }
    }

    public ArrayList<Belanja> FindItem(String findText){
        ArrayList<Belanja> findArray = new ArrayList<>();
        for (int index = 0; index<ItemSell.size(); index++){
            ArrayList<Belanja> itemSell = new ArrayList<>();
            Belanja item = new Belanja();
            if(findText.equals(ItemSell.get(index).getNamaBarang())){
                Belanja toFind = new Belanja();
                item.setHargaBarang(ItemSell.get(index).getHargaBarang());
                item.setHargaBarang(ItemSell.get(index).getHargaBarang());
                itemSell.add(item);

                toFind.setNamaBarang(getNamaBarang());
                toFind.setHargaBarang(getHargaBarang());
                toFind.setJumBelanja(getJumBelanja());
                toFind.setItemSell(itemSell);
                findArray.add(toFind);
            }
        }
        return findArray;
    }

    public static void main(String[] args) {
        int jum = 4;
        ArrayList<Belanja> p = new ArrayList<>();
        for (int index = 0; index < jum; index++){
            Belanja s = new Belanja();
            Scanner sc = new Scanner(System.in);
            System.out.print("Type Item Name :");
            s.setNamaBarang(sc.nextLine());
            System.out.print("Type Item Price :");
            s.setHargaBarang(sc.nextInt());
            System.out.print("Type Item QTY :");
            s.setJumBelanja(sc.nextInt());
            p.add(s);
        }
        System.out.print("-----------------------");
        System.out.format("Total Belanja : %60s");
        Belanja total = new Belanja();
        total.CetakInvoice(p);
