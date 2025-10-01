class GfG {

    static int longestUniqueSubstr(String s){
        int n = s.length();
        int res = 0;

        for (int i = 0; i < n; i++) {

            // Initializing all characters as not visited
            boolean[] vis = new boolean[26];

            for (int j = i; j < n; j++) {

                // If current character is visited
                // Break the loop
                if (vis[s.charAt(j) - 'a'] == true)
                    break;

                // Else update the result if this window is
                // larger, and mark current character as
                // visited.
                else {
                    res = Math.max(res, j - i + 1);
                    vis[s.charAt(j) - 'a'] = true;
                }
            }
        }
        return res;
    }

    public static void main(String[] args){
        String s = "geeksforgeeks";
        System.out.println(longestUniqueSubstr(s));
    }
}
