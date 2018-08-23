public class Solution {
    public int FirstUniqChar(string s) {
        Dictionary <char, int> myDict=new Dictionary<char, int>();
        Dictionary <char, int> myDict1=new Dictionary<char, int>();
        for (int i=97; i<123; i++){
            myDict.Add((char)i, 0);
            myDict1.Add((char)i, -1);
            
        }
        for (int i=0; i<s.Length; i++){
            myDict[s[i]]++;
            myDict1[s[i]]=i;            
        }
        
        
        foreach (KeyValuePair <char, int> pair in myDict){
            if(pair.Value!=1) myDict1.Remove(pair.Key);
        }
        List<int> myList=myDict1.Values.ToList();
        try{return myList.Min();}
        catch{return -1;}
    }
}
