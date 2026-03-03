public class OopsBanner {

    public static void main(String[] args) {
        renderBanner();
    }

    public static void renderBanner() {
        String[] bannerLines = {
            String.join("", " OOOO ", "  PPPP  ", "  PPPP  ", "  SSSS "),
            String.join("", "O    O", " P   P ", " P   P ", " S     "),
            String.join("", "O    O", " PPPP  ", " PPPP  ", "  SSS  "),
            String.join("", "O    O", " P     ", " P     ", "     S "),
            String.join("", " OOOO ", " P     ", " P     ", " SSSS  ")
        };

        for (String line : bannerLines) {
            System.out.println(line);
        }
    }
}
