public class Block {
    private int width;
    private int length;
    private int heigth;

    public int getWidth() {
        return width;
    }

    public int getLength() {
        return length;
    }

    public int getHeigth() {
        return heigth;
    }

    public Block(int[]arr) {
        this.width = arr[0];
        this.length = arr[1];
        this.heigth = arr[2];
    }

    public int getVolume(){
        return width * length * heigth;
    }

    public int getSurfaceArea(){
        return 2 * (width * length + width * heigth + length * heigth);
    }
}
