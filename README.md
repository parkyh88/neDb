# neDb
neDb 사용 예제

# create
neDb.insert<USER>(createData);
  
# find
neDb.find({ id: 0 }, { name: 'parkyh88' })
  
# find Pagination
const { pageNum, pageSize, param } = params; 
const skipCount = (pageNum - 1) * pageSize;
  
neDb.find({ id: 0 }, { name: 'parkyh88' })
  .find({ id: 0 }, { name: 'parkyh88' })
  .skip(skipCount)
  .limit(pageSize)
  .exec()
 
# update
neDb.update({ id: 0 }, { $set: { updatedAt : timestamp  }});

# delete
neDb.remove({ id: 0 }, {});
