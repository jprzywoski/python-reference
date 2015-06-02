os.chdir(path) 
os.getcwd() 
os.listdir(path) 
os.makedirs(path[, mode]) 
os.removedirs(path) 
os.renames(old, new) 
os.walk(top, topdown=True, onerror=None, followlinks=False)
os.startfile(path[, operation]) 


os.path.exists(path) 
os.path.join(path, *paths) 
os.path.split(path) 


shutil.copy2(src, dst) 
shutil.copytree(src, dst, symlinks=False, ignore=None) 
shutil.rmtree(path[, ignore_errors[, onerror]]) 
shutil.move(src, dst) 


shutil.make_archive(base_name, format[, root_dir[, base_dir[, verbose[, dry_run[, owner[, group[, logger]]]]]]]) 
ZipFile.extractall([path[, members[, pwd]]]) 
TarFile.extractfile(member) 

glob.glob(pathname) 
glob.iglob(pathname) 


