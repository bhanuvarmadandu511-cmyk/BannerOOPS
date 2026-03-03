public class OopsBanner {

    public static void main(String[] args) {
        renderBanner();
    }

    public static void renderBanner() {
        String[] oPattern = getOPattern();
        String[] pPattern = getPPattern();
        String[] sPattern = getSPattern();

        String[] bannerLines = new String[5];

        for (int i = 0; i < 5; i++) {
            bannerLines[i] = String.join("", oPattern[i], pPattern[i], pPattern[i], sPattern[i]);
        }

        for (String line : bannerLines) {
            System.out.println(line);
        }
    }

    public static String[] getOPattern() {
        return new String[]{
            " OOOO ",
            "O    O",
            "O    O",
            "O    O",
            " OOOO "
        };
    }

    public static String[] getPPattern() {
        return new String[]{
            "  PPPP  ",
            " P   P ",
            " PPPP  ",
            " P     ",
            " P     "
        };
    }

    public static String[] getSPattern() {
        return new String[]{
            "  SSSS ",
            " S     ",
            "  SSS  ",
            "     S ",
            " SSSS  "
        };
    }
}
