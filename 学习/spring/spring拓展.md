

@Autowired可以把所有的子类都加载上

例如：private List<BaseManager> list;

查找出所有的BaseManager子类，封装到list，原理是@Autowired会自动把相同类型的IUser对象收集到集合中。





