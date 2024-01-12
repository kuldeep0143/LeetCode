class Solution {
    public boolean halvesAreAlike(String str) {
        int n=str.length();
        int count=0;
        for(int i=0;i<n/2;i++){
            if(isVowel(str.charAt(i))){
                count++;
            }
        }
        for(int i=n/2;i<n;i++){
            if(isVowel(str.charAt(i))){
                count--;
            }
        }
        if(count==0){
            return true;
        }
        return false;
    }
    public boolean isVowel(char ch){
        if(ch=='a' ||ch=='e' ||ch=='i' ||ch=='o' ||ch=='u'
            ||ch=='A'||ch=='E' || ch=='I' || ch=='O' || ch=='U'){
                return true;
            }
            return false;
    }
}
