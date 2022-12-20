class BST:
  def __init__(self,key):
    self.key=key
    self.lchild=None
    self.rchild=None

  def insert(self,data):
    if self.key is None:
      self.key=data
      return
    if self.key==data:
      return
    if data<self.key:
      if self.lchild:
        self.lchild.insert(data)
      else:
        self.lchild=BST(data)
    else:
      if self.rchild:
        self.rchild.insert(data)
      else:
        self.rchild=BST(data)

  def search(self,data):
    if self.key==data:
      print('Node found')
      return
    if data<self.key:
      if self.lchild:
        self.lchild.search(data)
      else:
        print('Mode is not present in the tree')
    else:
      if self.rchild:
        self.rchild.search(data)
      else:
        print('Node is not present in the tree')

root=BST(10)
list=[6,3,4,8,9,2,0,1,7]
for i in list:
  root.insert(i)
root.search(4)
