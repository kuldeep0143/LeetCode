class Solution {
    public Node connect(Node node) {
        Map<Integer, List<Node>> map = new HashMap<>();
        goDFS(0, node, map);
        for (int key : map.keySet()) {
            List<Node> list = map.get(key);
            for (int i = 1; i < list.size(); i++) {
                list.get(i - 1).next = list.get(i);
            }
        }
        return node;
    }

    private void goDFS(int lvl, Node node, Map<Integer, List<Node>> map) {
        if (node == null) return;

        List<Node> list = map.computeIfAbsent(lvl, k -> new ArrayList<>());
        list.add(node);
        lvl++;
        goDFS(lvl, node.left, map);
        goDFS(lvl, node.right, map);
    }
}
